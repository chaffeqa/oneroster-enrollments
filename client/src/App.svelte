<script>
    import '../node_modules/materialize-css/dist/css/materialize.css';
    import '../node_modules/materialize-css/dist/js/materialize.min.js';

    import {Router, Route} from 'svelte-routing';
    import Navbar from './layout/Navbar.svelte';

    import Stats from './Stats.svelte';
    import School from './School.svelte';
    import Class from './Class.svelte';
    import Teacher from './User/Teacher.svelte'
    import Student from './User/Student.svelte';
</script>

<style>

</style>

<Router>
    <Navbar />
    <div class="container">
        <Route path="/" component={Stats}/>
        <Route path="/schools" component={School}/>
        <Route path="/classes" component={Class}/>
        <Route path="/teachers" component={Teacher}/>
        <Route path="/students" component={Student}/>
    </div>
</Router>


