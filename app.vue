<template>
    <div>
        <div
            class="
                uk-light
                wrap
                uk-background-norepeat
                uk-background-cover
                uk-background-center-center
                uk-cover-container
                uk-background-secondary
            "
        >
            <img
                data-srcset="https://picsum.photos/640/700/?random 640w,
                              https://picsum.photos/960/700/?random 960w,
                              https://picsum.photos/1200/900/?random 1200w,
                              https://picsum.photos/2000/1000/?random 2000w"
                sizes="100vw"
                data-src="https://picsum.photos/1200/900/?random"
                alt="Background"
                data-uk-cover
                data-uk-img
            />
            <div
                class="
                    uk-flex
                    uk-flex-center
                    uk-flex-middle
                    uk-height-viewport
                    uk-position-z-index
                    uk-position-relative
                "
                data-uk-height-viewport="min-height: 400"
                style="background-color: rgba(0, 0, 0, 0.5)"
            >
                <!-- Nav -->
                <div class="uk-position-top">
                    <div class="uk-container uk-container-small">
                        <nav
                            class="uk-navbar-container uk-navbar-transparent"
                            data-uk-navbar
                        >
                            <div class="uk-navbar-left">
                                <div class="uk-navbar-item">
                                    <NuxtLink to="/" class="uk-logo">
                                        <img src="/uikit.svg" alt="Logo" />
                                    </NuxtLink>
                                </div>
                            </div>
                            <div class="uk-navbar-right">
                                <ul class="uk-navbar-nav">
                                    <li class="uk-visible@s">
                                        <NuxtLink to="">Home</NuxtLink>
                                    </li>
                                    <li class="uk-visible@s">
                                        <NuxtLink to="">About</NuxtLink>
                                    </li>
                                    <li class="uk-visible@s">
                                        <NuxtLink to="">Contact</NuxtLink>
                                    </li>
                                    <li>
                                        <a
                                            class="uk-navbar-toggle"
                                            data-uk-toggle
                                            data-uk-navbar-toggle-icon
                                            href="#offcanvas-nav"
                                        ></a>
                                    </li>
                                </ul>
                            </div>
                        </nav>
                    </div>
                </div>
                <!-- Content -->
                <div
                    class="
                        uk-container
                        uk-container-small
                        uk-flex-auto
                        uk-text-center
                    "
                    data-uk-scrollspy="target: > .animate; cls: uk-animation-slide-bottom-small uk-invisible; delay: 300"
                >
                    <h1 class="uk-heading-prinary animate uk-invisible">
                        UIkit + Nuxt =
                        <span data-uk-icon="icon: heart; ratio: 2.5;"></span>
                    </h1>
                    <div
                        class="
                            uk-width-4-5@m uk-margin-auto
                            animate
                            uk-invisible
                        "
                    >
                        <p class="lead">
                            Lorem ipsum dolor sit amet, consectetur adipisicing
                            elit. A ad, reiciendis maxime, facilis nam natus
                            incidunt provident.
                        </p>
                    </div>
                    <div
                        class="uk-margin-medium-top animate uk-invisible"
                        data-uk-margin
                        data-uk-scrollspy-class="uk-animation-fade uk-invisible"
                    >
                        <a
                            class="
                                uk-button
                                uk-button-default
                                uk-button-large
                                uk-width-2-3
                                uk-width-auto@s
                            "
                            data-uk-icon="arrow-right"
                            title="Learn More"
                            target="_blank"
                            href="https://github.com/fedorae-com/nuxt-uikit"
                        >
                            LEARN MORE
                        </a>
                        <a
                            class="
                                uk-margin-small-left
                                uk-button
                                uk-button-primary
                                uk-button-large
                                uk-width-2-3
                                uk-width-auto@s
                            "
                            data-uk-icon="check"
                            title="Try it out"
                            target="_blank"
                            href="https://nuxt-uikit.fedorae.com"
                        >
                            TRY IT OUT
                        </a>
                    </div>
                </div>

                <!-- Footer -->
                <div class="uk-position-bottom-center uk-position-small">
                    <span class="uk-text-small uk-text-center">
                        &copy; 2023 Fedorae |
                        <a
                            href="https://github.com/zzseba78/Kick-Off"
                            title="Inspired by KickOff"
                            target="_blank"
                        >
                            Inspired by KickOff
                        </a>
                        | Built with
                        <a
                            href="http://getuikit.com"
                            title="Visit UIkit 3 site"
                            target="_blank"
                            data-uk-tooltip
                        >
                            <span data-uk-icon="uikit"></span>
                        </a>
                        &
                        <a
                            href="http://nuxt.com"
                            title="Visit Nuxt site"
                            target="_blank"
                            data-uk-tooltip
                        >
                            <span
                                class="uk-icon uk-icon-image"
                                style="background-image: url(/nuxt.svg)"
                            ></span>
                        </a>
                    </span>
                </div>
            </div>
        </div>

        <!-- Offcanvas -->
        <div id="offcanvas-nav" data-uk-offcanvas="flip: true; overlay: false">
            <div
                class="
                    uk-offcanvas-bar
                    uk-offcanvas-bar-animation
                    uk-offcanvas-slide
                "
            >
                <button
                    class="uk-offcanvas-close uk-close uk-icon"
                    type="button"
                    data-uk-close
                ></button>
                <ul class="uk-nav uk-nav-default">
                    <li class="uk-active"><a href="#">Active</a></li>
                    <li class="uk-parent">
                        <a href="#">Parent</a>
                        <ul class="uk-nav-sub">
                            <li><a href="#">Sub item</a></li>
                            <li><a href="#">Sub item</a></li>
                        </ul>
                    </li>
                    <li class="uk-nav-header">Header</li>
                    <li>
                        <a href="#">
                            <span
                                class="uk-margin-small-right uk-icon"
                                data-uk-icon="icon: table"
                            ></span>
                            Item
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <span
                                class="uk-margin-small-right uk-icon"
                                data-uk-icon="icon: thumbnails"
                            ></span>
                            Item
                        </a>
                    </li>
                    <li class="uk-nav-divider"></li>
                    <li>
                        <a href="#">
                            <span
                                class="uk-margin-small-right uk-icon"
                                data-uk-icon="icon: trash"
                            >
                            </span>
                            Item
                        </a>
                    </li>
                </ul>
                <h3>Title</h3>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris nisi ut aliquip ex ea commodo consequat.
                </p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.uk-logo img {
    height: 28px;
}
</style>
