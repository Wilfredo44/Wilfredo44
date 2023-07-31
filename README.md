- void setup() {
  size(400, 400); // Tamaño de la ventana de dibujo
  background(220, 220, 255); // Fondo celeste claro
}

void draw() {
  // Cuerpo del loro
  fill(255, 165, 0); // Color naranja
  stroke(0); // Color del borde (negro)
  ellipse(200, 250, 150, 150); // Cuerpo

  // Cabeza del loro
  fill(255, 255, 0); // Color amarillo
  ellipse(120, 180, 100, 100); // Cabeza

  // Ojos
  fill(0); // Color negro
  ellipse(100, 170, 20, 20); // Ojo izquierdo
  ellipse(140, 170, 20, 20); // Ojo derecho

  // Pico
  fill(255, 140, 0); // Color naranja oscuro
  triangle(140, 190, 160, 190, 150, 210); // Pico

  // Patas
  strokeWeight(8); // Grosor de las patas
  line(180, 280, 180, 350); // Pata izquierda
  line(220, 280, 220, 350); // Pata derecha

  // Cola
  fill(0, 255, 0); // Color verde
  beginShape();
  vertex(220, 200);
  vertex(270, 180);
  vertex(250, 230);
  endShape(CLOSE);
}
