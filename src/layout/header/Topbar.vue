<template>
  <!--begin::Toolbar wrapper-->
  <div class="d-flex align-items-stretch flex-shrink-0">
    <!--begin::Search-->
    <div class="d-flex align-items-stretch ms-1 ms-lg-3">
      <KTSearch></KTSearch>
    </div>
    <!--end::Search-->

    <!--begin::Chat-->
    <!-- <div class="d-flex align-items-center ms-1 ms-lg-3">
    <div class="
          btn btn-icon btn-active-light-primary
          position-relative
          w-30px
          h-30px
          w-md-40px
          h-md-40px
        " id="kt_drawer_chat_toggle">
      <span class="svg-icon svg-icon-1">
        <inline-svg src="media/icons/duotune/communication/com012.svg" />
      </span>

      <span class="
            bullet bullet-dot
            bg-success
            h-6px
            w-6px
            position-absolute
            translate-middle
            top-0
            start-50
            animation-blink
          ">
      </span>
    </div> 
  </div>-->
    <!--end::Chat-->

    <!--begin::User-->
    <!-- <div
      class="d-flex align-items-center ms-1 ms-lg-3"
      id="kt_header_user_menu_toggle"
    >
      <MenuComponent menu-selector="#kt-user-menu">
        <template v-slot:toggle>
          <div
            class="
              cursor-pointer
              symbol symbol-circle symbol-30px symbol-md-40px
            "
            data-kt-menu-target="#kt-user-menu"
            data-kt-menu-trigger="click"
            data-kt-menu-attach="parent"
            data-kt-menu-placement="bottom-end"
            data-kt-menu-flip="bottom"
          >
            <img alt="Pic" src="media/avatars/150-1.jpg" />
          </div>
        </template>
        <template v-slot:content>
          <KTUserMenu></KTUserMenu>
        </template>
      </MenuComponent>
    </div> -->
    <!--end::User -->
  </div>
  <!--end::Toolbar wrapper-->
</template>

<script lang="ts">
import { defineComponent } from "vue";
import KTSearch from "@/layout/header/partials/Search.vue";

export default defineComponent({
  name: "topbar",
  components: {
    // KTUserMenu,
    // KTNotificationMenu,
    KTSearch,
    // MenuComponent,
  },
});
</script>
