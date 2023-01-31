<template>
    <div>
        <header>
            <h1>{{theTitle}}</h1>
            <LinkButton />
        </header>
    </div>
</template>

<script>
import LinkButton from './LinkButton';

export default{
  components: { LinkButton },
    name: 'AppsHeader',
    props: ['theTitle'],
}

</script>

<style scoped>
    header{
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        margin-bottom: 20px;
        color: darkslateblue;
    }
</style>