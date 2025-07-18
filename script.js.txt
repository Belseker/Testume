function startTest() {
  const name = document.getElementById('name').value.trim();
  const baremo = parseFloat(document.getElementById('baremo').value);
  const testType = parseInt(document.getElementById('testType').value);
  const options = parseInt(document.getElementById('optionsCount').value);

  if (!name || isNaN(baremo) || isNaN(testType) || isNaN(options)) {
    alert('Por favor, completa todos los campos correctamente.');
    return;
  }

  document.getElementById('output').innerHTML =
    `✅ Bienvenido, ${name}.<br>
     🧠 Baremo: ${baremo}<br>
     📄 Test: ${testType} preguntas<br>
     🔢 Opciones por pregunta: ${options}<br><br>
     ¡Listo para empezar!`;
}
