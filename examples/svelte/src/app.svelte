<script>
    
import { Datagrid } from '@activewidgets/svelte';
import './styles.css';

let rows = [
    { message: 'Hello, World!' }
];

</script>

<Datagrid {rows} />