<script>
  import { Router, Route, useParams} from "svelte-navigator";
  import Navbar from "./components/Navbar.svelte";
  import Home from "./routes/Home.svelte";
  import All from "./routes/All.svelte";
  import Game from "./routes/Game.svelte";
  import Character from "./routes/Character.svelte";
//import Character from "./routes/Character.svelte";
  
  //let id = {params._id}
  
  </script>
  
  <Router>
    <Navbar />
  
    <div>
      <Route path="/">
        <Home />
      </Route>
      <Route path="/all">
        <All />
      </Route>
       <Route path="all/:id" let:params>
        <Character id={params.id}/>
      </Route>
      <Route path="/game">
        <Game />
      </Route>
      

  
     
  
    </div>
  
  </Router>