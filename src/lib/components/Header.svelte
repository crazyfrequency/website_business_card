<script lang="ts">
    import logo from "$lib/images/logo.png";
    import * as Popover from "$lib/components/ui/popover";
    import { Button } from "$lib/components/ui/button";
</script>

<div class="flex mx-3 md:mx-14 lg:mx-16 xl:mx-28 my-11 justify-between">
    <img src={logo} alt="#" class="h-12 md:h-14 lg:h-20 xl:h-24" />
    <nav class="hidden md:flex gap-4 lg:gap-8 xl:gap-12 2xl:gap-16">
        <a href="@" class="self-center font-montserrat lg:text-lg xl:text-2xl 2xl:text-4xl font-normal text-[#A7CAE9]">Возможности</a>
        <a href="@" class="self-center font-montserrat lg:text-lg xl:text-2xl 2xl:text-4xl font-normal text-[#A7CAE9]">Проекты</a>
        <a href="@" class="self-center font-montserrat lg:text-lg xl:text-2xl 2xl:text-4xl font-normal text-[#A7CAE9]">Отзывы</a>
        <a href="@" class="self-center font-montserrat lg:text-lg xl:text-2xl 2xl:text-4xl font-normal text-[#A7CAE9]">Контакты</a>
    </nav>
    <Popover.Root>
        <Popover.Trigger asChild let:builder>
            <Button builders={[builder]} class="md:hidden" variant="outline" size="icon">
                <svg xmlns="http://www.w3.org/2000/svg" class="size-14" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M4 6l16 0"/>
                    <path d="M4 12l16 0" />
                    <path d="M4 18l16 0" />
                </svg>
            </Button>
        </Popover.Trigger>
        <Popover.Content class="grid grid-rows-4 gap-7 w-80 bg-[#191333]">
            <a href="@" class="self-center font-montserrat text-2xl text-[#A7CAE9]">Возможности</a>
            <a href="@" class="self-center font-montserrat text-2xl text-[#A7CAE9]">Проекты</a>
            <a href="@" class="self-center font-montserrat text-2xl text-[#A7CAE9]">Обзоры</a>
            <a href="@" class="self-center font-montserrat text-2xl text-[#A7CAE9]">Контакты</a>
        </Popover.Content>
    </Popover.Root>
</div>

