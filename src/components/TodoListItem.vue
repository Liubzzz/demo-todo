<script setup>
defineProps({
    id: Number,
    title: String,
    completed: Boolean
})





</script>

<template>
<div class="grid-container">
    <div class ="grid-item"><input type="checkbox"  id="toggle" :checked="completed" /></div>
   <div class="grid-item">{{ title }}</div>
    <div class="grid-item">







<button class="button-33" role="button">Delete</button>









    </div>
    </div>


<!-- <h1>Grid Layout</h1> -->

<!-- <p>This grid layout contains six columns and three rows:</p>

<div class="grid-container">
  <div class="item1">Header</div>
  <div class="item2">Menu</div>
  <div class="item3">Main</div>  
  <div class="item4">Right</div>
  <div class="item5">Footer</div>
</div> -->

</template>

<style scoped>




/* .item1 { grid-area: header; }
.item2 { grid-area: menu; }
.item3 { grid-area: main; }
.item4 { grid-area: right; }
.item5 { grid-area: footer; }

.grid-container {
  display: grid;
  grid-template-areas:
    'header header header header header header'
    'menu main main main right right'
    'menu footer footer footer footer footer';
  gap: 10px;
  background-color: #2196F3;
  padding: 10px;
}

.grid-container > div {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px 0;
  font-size: 30px;
} */





.grid-container {
    display:grid;
    column-gap: 50px;
     row-gap: 150px; 
  grid-template-columns: 1fr 1fr 1fr;
  background-color: #2196F3;
  padding: 10px;
}
.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  border: 1px solid rgba(0, 0, 0, 0.8);
  padding: 20px;
  font-size: 30px;
  text-align: center;
}

div {
  text-align: justify;
  text-justify: inter-word;
}





/* CSS */
.button-33 {
  background-color: #c2fbd7;
  border-radius: 100px;
  box-shadow: rgba(50, 187, 99, .2) 0 -25px 18px -14px inset,rgba(44, 187, 99, .15) 0 1px 2px,rgba(44, 187, 99, .15) 0 2px 4px,rgba(44, 187, 99, .15) 0 4px 8px,rgba(44, 187, 99, .15) 0 8px 16px,rgba(44, 187, 99, .15) 0 16px 32px;
  color: black;
  cursor: pointer;
  display: inline-block;
  font-family: CerebriSans-Regular,-apple-system,system-ui,Roboto,sans-serif;
  padding: 7px 20px;
  text-align: center;
  text-decoration: none;
  transition: all 250ms;
  border: 0;
  font-size: 16px;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.button-33:hover {
  box-shadow: rgba(44,187,99,.35) 0 -25px 18px -14px inset,rgba(44,187,99,.25) 0 1px 2px,rgba(44,187,99,.25) 0 2px 4px,rgba(44,187,99,.25) 0 4px 8px,rgba(44,187,99,.25) 0 8px 16px,rgba(44,187,99,.25) 0 16px 32px;
  transform: scale(1.05) rotate(-1deg);
}








:root {
  --body: #fafafa;
  --text-default: #1d1d1f;
  --text-secondary: #86868b;
}
@media (prefers-color-scheme: light) {
  :root {
    --body: #fafafa;
    --text-default: #1d1d1f;
  }
}
@media (prefers-color-scheme: dark) {
  :root {
    --body: #161616;
    --text-default: #f5f5f7;
  }
}
body {
  height: 50vh;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  background-color: var(--body);
}
/* Checkbox Styles */
input[type="checkbox"] {
  -webkit-appearance: none;
  outline: none;
  position: absolute;
  height: 3rem;
  width: 4rem;
  border: 3px solid var(--body);
  border-radius: 2.5rem;
  cursor: pointer;
  box-shadow: 9px 9px 16px rgba(189, 189, 189, 0.6), -9px -9px 16px rgba(255, 255, 255, 0.5), inset 10px 10px 15px -10px #c3c3c3, inset -10px -10px 15px -10px #fff;
  /* Toggle Indicator */
  /* Label */
  /* Checked Styles */
}
@media (prefers-color-scheme: light) {
  input[type="checkbox"] {
    box-shadow: 4px 4px 10px rgba(189, 189, 189, 0.6), -9px -9px 16px rgba(255, 255, 255, 0.5), inset 10px 10px 15px -10px #c3c3c3, inset -10px -10px 15px -10px #fff;
  }
}
@media (prefers-color-scheme: dark) {
  input[type="checkbox"] {
    box-shadow: -8px -4px 8px 0px rgba(255, 255, 255, 0.05), 8px 4px 12px 0px rgba(0, 0, 0, 0.5), inset -4px -4px 4px 0px rgba(255, 255, 255, 0.05), inset 4px 4px 4px 0px rgba(0, 0, 0, 0.5);
  }
}
input[type="checkbox"]::before {
  content: "";
  height: 3.125rem;
  width: 3.125rem;
  background-color: var(--body);
  position: absolute;
  margin: auto;
  top: 0;
  left: 0.9375rem;
  bottom: 0;
  border-radius: 50%;
  box-shadow: 7px 7px 15px #c3c3c3, 9px 9px 16px rgba(189, 189, 189, 0.6);
  transition: 0.15s;
}
@media (prefers-color-scheme: light) {
  input[type="checkbox"]::before {
    box-shadow: 7px 7px 15px #c3c3c3, 9px 9px 16px rgba(189, 189, 189, 0.6);
  }
}
@media (prefers-color-scheme: dark) {
  input[type="checkbox"]::before {
    box-shadow: -8px -4px 8px 0px rgba(255, 255, 255, 0.05), 8px 4px 12px 0px rgba(0, 0, 0, 0.5);
  }
}
input[type="checkbox"]::after {
  content: "Off";
  position: absolute;
  font-size: 1.625rem;
  top: 1.25rem;
  right: 1.5625rem;
  color: var(--text-secondary);
  font-family: "SF Pro Text", "Helvetica Neue", "Helvetica", "Arial", sans-serif;
  font-weight: 400;
  letter-spacing: 0.004em;
}
input[type="checkbox"]:checked {
  background: #0071e3;
}
@media (prefers-color-scheme: light) {
  input[type="checkbox"]:checked {
    box-shadow: 9px 9px 16px rgba(189, 189, 189, 0.6), -9px -9px 16px rgba(255, 255, 255, 0.5), inset 10px 10px 15px -10px #0047b9, inset -10px -10px 15px -10px #0047b9;
  }
}
input[type="checkbox"]:checked::before {
  left: 5.3125rem;
  box-shadow: none;
}
input[type="checkbox"]:checked::after {
  content: "On";
  left: 1.5625rem;
  color: #f5f5f7;
}






</style>






