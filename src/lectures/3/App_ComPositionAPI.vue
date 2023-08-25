```jsx
<script setup>
import { onMounted, reactive, ref } from 'vue';

const counter = ref(0);
// eslint-disable-next-line no-unused-vars
const increment = () => {
	counter.value++;
};

const books = reactive([]);
// eslint-disable-next-line no-unused-vars
const addBook = (title, author) => {
	books.push({ title, author });
};

onMounted(() => {
	console.log('애플리케이션이 마운트 되었습니다!');
});
</script>
