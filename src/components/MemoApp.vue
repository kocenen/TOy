<template>
    <div class = 'memo-app'>
        <memo-form></memo-form>
        <memo></memo>
    </div>
</template>

<script>
import MemoForm from '@/components/MemoForm';
import MemoApp from '@/components/MemoApp';
    
export default {
    name : 'MemoApp',
    data(){
        return{
            memoArr: [],
        };
    },
    created(){
        this.memoArr = localStorage.memos? Json.parse(localStorage.memos) : [];
    }
}
</script>