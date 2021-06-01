<template>
  <div>
  </div>
</template>

<script>
import Octocat from '@/octocat.js'

export default {
  name: 'Octocat',
  mounted() {   
    const script = function (p5) {    
      let octocat

      // NOTE: Set up is here   
      p5.setup = () => {      
        p5.createCanvas(500, 500);      
        octocat = new Octocat();
        octocat.setBodyColor({ primary: "#282828", underside: "#494949", suctions: "#99C7C9" })
				//CODE_HERE
      }     
      
      // NOTE: Draw is here
      p5.draw = () => {    
        p5.background("white")
        octocat.draw(p5)
      }  
    }

    // NOTE: Use p5 as an instance mode
    const P5 = require('p5');
    new P5(script)
  }
}
</script>
