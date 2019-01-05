<template>
    <div class="mobileWrapper">
        <header class="mobileWrapper__header">
            <a href="#">
                <i class="fas fa-long-arrow-alt-left"></i>
                Back
            </a>
            <h1>Flexbox app layout</h1>
            <a href="#">
                <i class="fab fa-whmcs"></i>
            </a>
        </header>
        <section class="mobileWrapper__content">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit?</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod corporis dolore repudiandae autem ea magni, distinctio recusandae assumenda hic exercitationem possimus cum perspiciatis ratione nam laudantium culpa consequuntur. Non, tempora?</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ducimus delectus magnam nam adipisci excepturi soluta labore vero dolor laudantium ratione eveniet id vel asperiores, optio aperiam perferendis minima voluptates voluptatem.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste aliquid temporibus praesentium fugiat dignissimos, officia repellat beatae mollitia ea nihil.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, illo magnam ipsa sint eum autem iste ipsum, veritatis dolores voluptate praesentium sunt aliquam quis aspernatur! Rem sed quis ratione et.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque in eaque voluptatibus ullam eligendi? Repellat harum dolorem eos inventore quia pariatur ullam voluptate. Porro sequi suscipit voluptate doloremque fugit cupiditate?</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit?</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quod corporis dolore repudiandae autem ea magni, distinctio recusandae assumenda hic exercitationem possimus cum perspiciatis ratione nam laudantium culpa consequuntur. Non, tempora?</p>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ducimus delectus magnam nam adipisci excepturi soluta labore vero dolor laudantium ratione eveniet id vel asperiores, optio aperiam perferendis minima voluptates voluptatem.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iste aliquid temporibus praesentium fugiat dignissimos, officia repellat beatae mollitia ea nihil.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, illo magnam ipsa sint eum autem iste ipsum, veritatis dolores voluptate praesentium sunt aliquam quis aspernatur! Rem sed quis ratione et.</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Neque in eaque voluptatibus ullam eligendi? Repellat harum dolorem eos inventore quia pariatur ullam voluptate. Porro sequi suscipit voluptate doloremque fugit cupiditate?</p>
        </section>
        <div class="mobileWrapper__iconBar">
            <a href="#">
                <i class="fas fa-home"></i>
                Home
            </a>
            <a href="#">
                <i class="fas fa-bell"></i>
                Notifications
            </a>
            <a href="#">
                <i class="fas fa-comment"></i>
                Messages
            </a>
            <a href="#">
                <i class="fas fa-user"></i>
                Me
            </a>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .mobileWrapper {
        width: 400px;
        border: 10px solid black;
        border-bottom: 50px solid black;
        border-radius: 4px;

        display: flex;
        flex-direction: column;

        & > * {
            flex: 1 1 auto;
        }

        &__header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 20px 10px;
            background-color: #e6c839;

            h1 {
                font-size: 24px;
                text-transform: capitalize;
            }

            a {
                &,
                &:link,
                &:visited {
                    padding: 4px 8px;
                    border-radius: 4px;
                    color: #fff;
                    background-color: rgba(0,0,0,.1);
                    text-decoration: none;
                }

                &:hover {
                    background-color: rgba(0,0,0,.2);
                }
            }
        }

        &__content {
            height: 500px;
            background-color: #fff;
            overflow-y: scroll;
        }

        &__iconBar {
            display: flex;
            background-color: #e6c839;

            a {
                &,
                &:link,
                &:visited {
                    flex: 1;
                    display: inline-block;
                    position: relative;
                    padding: 14px 8px;
                    border-radius: 4px;
                    border-right: 1px solid rgba(0,0,0, .1);
                    font-size: 12px;
                    text-align: center;
                    text-decoration: none;
                    color: #000;
                }

                &::after {
                    position: absolute;
                    bottom: 0;
                    left: 0;

                    content: '';
                    width: 100%;
                    height: 8px;
                    background-color: transparent;

                    transition: all .3s;
                }

                &:hover::after {
                    background-color: rgba(0,0,0,.4);
                }


            & > * {
                display: block;
                margin-bottom: 8px;
            }

            & > i {
                font-size: 18px;
                color: #fff;
            }
        }
    }
}
</style>
