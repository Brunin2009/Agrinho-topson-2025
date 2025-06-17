function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
}
let angle = 0;

function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  
  translate(width / 2, height / 2); // Move a origem para o centro da tela
  rotate(angle); // Aplica a rotação
  
  // Desenha o rosto
  fill(255, 204, 0); // Cor do rosto
  ellipse(0, 0, 150, 150); // Rosto
  
  // Olhos
  fill(0); // Cor dos olhos
  ellipse(-40, -20, 20, 20); // Olho esquerdo
  ellipse(40, -20, 20, 20); // Olho direito
  
  // Sorriso
  noFill();
  stroke(0);
  strokeWeight(4);
  arc(0, 20, 80, 80, 0, PI); // Sorriso
  
  angle += 0.01; // Aumenta o ângulo para girar
}
