<template>
  <main class="container cart">
    <h2>Cart</h2>

    <section>
      <table>
        <thead>
          <tr>
            <th>Item</th>
            <th>Add Ons</th>
            <th>Amount</th>
            <th>Total Price</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>
              <span></span>
            </td>
            <td>
              <span class="comma"></span>
            </td>
            <td></td>
            <td></td>
          </tr>
          <tr>
            <td colspan="3"></td>
            <td class="total">Total: 14</td>
          </tr>
        </tbody>
      </table>
    </section>
  </main>
</template>

<script>
import { mapState } from 'vuex'

export default {
  name: 'cartPage',

  computed: {
    ...mapState(['cart'])
  }
}
</script>

<style lang="scss" scoped></style>
