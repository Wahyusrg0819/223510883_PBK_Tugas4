<template>
  <div class="modal-overlay" @click.self="$emit('close')">
    <div class="modal-content" >
      <h3>Kontak Saya</h3>
      <p>Nama: Wahyu Muliadi Siregar</p>
      <p>Email: wahyumuliadisiregar@student.uir.ac.id</p>
      <p>Telepon: +62 85763304788</p>
      <button @click="closeContactModal">Close</button>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ContactModal'
};
</script>

<style scoped>
.modal-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}
.modal-content {
  background: white;
  padding: 20px;
  border-radius: 5px;
}

button {
  padding: 1.3em 3em;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: 2.5px;
  font-weight: 500;
  color: #000;
  background-color: #fff;
  border: none;
  border-radius: 45px;
  box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease 0s;
  cursor: pointer;
  outline: none;
  margin-top: 3%;
  margin-bottom: 3%;
}

button:hover {
  background-color: #23c483;
  box-shadow: 0px 15px 20px rgba(46, 229, 157, 0.4);
  color: #fff;
  transform: translateY(-7px);
}

button:active {
  transform: translateY(-1px);
}
</style>
