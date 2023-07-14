# Qwerty-keyboard

<div id="qwerty" class="section">
    <div class="keyrow">
      <button>q</button><button>w</button><button>e</button><button>r</button>
      <button>t</button><button>y</button><button>u</button><button>i</button> 
      <button>o</button><button>p</button>
    </div>
    <div class="keyrow">
      <button>a</button><button>s</button><button>d</button><button>f</button> 
      <button>g</button><button>h</button><button>j</button><button>k</button>
      <button>l</button>
    </div>
    <div class="keyrow">
      <button>z</button><button>x</button><button>c</button><button>v</button> 
      <button>b</button><button>n</button><button>m</button>
    </div>
</div>

<input id="input" />

var input = document.querySelector('#input')

document.querySelectorAll('#qwerty button').forEach(el => {
  el.addEventListener('click', () => {
    input.value = input.value + el.innerText
  })
})
