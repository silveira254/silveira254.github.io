body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

header {
  background-color: #ff69b4;
  color: white;
  padding: 20px;
  text-align: center;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  padding: 0;
}

nav ul li {
  margin: 0 15px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

.produtos {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin: 30px;
}

.produto {
  border: 1px solid #ccc;
  padding: 15px;
  margin: 10px;
  text-align: center;
  width: 200px;
}

.produto img {
  max-width: 100%;
}

button {
  background-color: #ff69b4;
  color: white;
  border: none;
  padding: 10px;
  cursor: pointer;
}

button:hover {
  background-color: #ff1493;
}

footer {
  background-color: #f2f2f2;
  text-align: center;
  padding: 15px;
  margin-top: 40px;
}
let carrinhoContador = 0;

function adicionarCarrinho(produto) {
  carrinhoContador++;
  alert(produto + " adicionado ao carrinho!");
  document.getElementById("carrinho").textContent = `Carrinho (${carrinhoContador})`;
}
