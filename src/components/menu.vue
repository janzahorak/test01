<template>
  <div class="menu">
      <div class="menu__item bg-gray">
        <div class="menu__content">
          <div class="m-toggle">
              <input type="checkbox" id="m-toggle-item-1" name="m-toggle[]" aria-hidden="true" class="m-toggle__control sr-only">
              <label class="m-toggle__label" for="m-toggle-item-1">
                  <span class="m-toggle__title">Hlavní jídlo</span>
                  <span class="m-toggle__arrow">
                      <i class="a-icon-angle-right" aria-hidden="true"></i>
                  </span>
              </label>
              <div class="m-toggle__panel">
                  <div class="m-toggle__content">
                      <ul>
                          <li>
                            <p>Totopos con salsa y guacamole</p>
                            <span>139,-</span>
                          </li>
                          <li>
                            <p>Totopos con salsa y guacamole</p>
                            <span>139,-</span>
                          </li>
                          <li>
                            <p>Totopos con salsa y guacamole</p>
                            <span>139,-</span>
                          </li>
                          <li>
                            <p>Totopos con salsa y guacamole</p>
                            <span>139,-</span>
                          </li>
                      </ul>
                  </div>
              </div>
          </div>
          <div class="m-toggle">
              <input type="checkbox" id="m-toggle-item-2" name="m-toggle[]" aria-hidden="true" class="m-toggle__control sr-only">
              <label class="m-toggle__label" for="m-toggle-item-2">
                  <span class="m-toggle__title">Přílohy</span>
                  <span class="m-toggle__arrow">
                      <i class="a-icon-angle-right" aria-hidden="true"></i>
                  </span>
              </label>
              <div class="m-toggle__panel">
                  <div class="m-toggle__content">
                      <ul>
                          <li>Guacamoleee</li>
                          <li>Pico de gallo</li>
                          <li>Tortilla de Maiz</li>
                          <li>Tortilla de Harina</li>
                      </ul>
                  </div>
              </div>
          </div>
          <div class="m-toggle">
              <input type="checkbox" id="m-toggle-item-3" name="m-toggle[]" aria-hidden="true" class="m-toggle__control sr-only">
              <label class="m-toggle__label" for="m-toggle-item-3">
                  <span class="m-toggle__title">Nápoje</span>
                  <span class="m-toggle__arrow">
                      <i class="a-icon-angle-right" aria-hidden="true"></i>
                  </span>
              </label>
              <div class="m-toggle__panel">
                  <div class="m-toggle__content">
                      <ul>
                          <li>Perlivá, neperlivá voda</li>
                          <li>Kofola, Coca-Cola</li>
                          <li>Agua fresca/domácí limonáda</li>
                          <li>Jumex džus / juice</li>
                      </ul>
                  </div>
              </div>
          </div>
        </div>
      </div>
      <div class="menu__item">
      </div>
  </div>
</template>

<script>
export default {
  name: 'menu',
  data () {
    return {
      menu: [
        {
          title: 'Hlavní jídlo',
          items: [
            {
              name: 'Totopos con salsa y guacamole',
              description: 'Kukuřičné tortilla cipsy s guacamole a omáčkou dle výběru.',
              price: 139
            },
            {
              name: 'TOTOPOS CON SALSA',
              description: 'Kukuřičné tortilla cipsy s guacamole a omáčkou dle výběru.',
              price: 79
            }
          ]
        },
        {
          title: 'Přílohy',
          items: [
            {
              name: 'Guacamole 50g / 150g',
              description: null,
              price: 79
            },
            {
              name: 'Pico de gallo 50g / 150g',
              description: null,
              price: 79
            }
          ]
        },
        {
          title: 'Nápoje',
          items: [
            {
              name: 'Perlivá, neperlivá voda (0,5l)',
              description: null,
              price: 35
            },
            {
              name: 'Kofola, Coca-Cola (0,5l)',
              description: null,
              price: 35
            }
          ]
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.bg-gray {
  background-color: #f6f6f6;
}

.menu {
  display: flex;
}

.menu__item {
    flex: 0 0 50%;
    max-width: 50%;
}

.menu__content {
  display: flex;
  flex-direction: column;
  height: 100%;
  margin: 40px;
}

.m-toggle {
    display: flex;
    flex-direction: column;
    align-items: baseline
}

.m-toggle + .m-toggle {
    margin-top: 10px;
}

.m-toggle__label {
    cursor: pointer;
    display: flex;
    flex-wrap: wrap;
    margin: 0;
    padding: 10px 20px;
    font-size: 18px;
    font-weight: bold;
}

.m-toggle__control {
  display: none;
}

.m-toggle__title {
    align-self: center;
    flex-basis: 0;
    flex-grow: 1;
    margin: 0;
    max-width: 100%;
}

.m-toggle__panel {
    display: block;
    height: auto;
    max-height: 0;
    overflow-y: hidden;
    transition: max-height .5s ease-out;
    width: 100%;
}

.m-toggle__content {
    border-top: 1px solid color('gray');
    padding: space(2);
}

.m-toggle__control:checked + .m-toggle__label + .m-toggle__panel {
    max-height: 80rem;
}

ul {
    margin: 0;
    list-style: none;
    text-align: left;
}

li {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 10px;
    border-bottom: dotted #e4e4e4;
}

li p {
  margin: 0;
}

</style>
