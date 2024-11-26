# cmas
// la clase
class Motor {
private:
int potencia;
public:
void encender() {
cout << "Motor encendido" << endl;
}
void setPotencia(int p) {
potencia = p;
}
void mostrarPotencia() {
cout << "Potencia del motor: " << potencia << " caballos de fuerza" << endl;
}
};

// segunda clase 
class Ruedas {
private:
int tamaño;
public:
void rodar() {
cout << "Las ruedas están rodando" << endl;
}
void setTamaño(int t) {
tamaño = t;
}
void mostrarTamaño() {
cout << "Tamaño de las ruedas: " << tamaño << " pulgadas" << endl;
}
};

// tercera clase 
class Coche {
private:
Motor motor;
Ruedas ruedas;
public:
void conducir() {
motor.encender();
ruedas.rodar();
cout << "El coche está en movimiento" << endl;
}
void setDetalles(int potencia, int tamaño) {
motor.setPotencia(potencia);
ruedas.setTamaño(tamaño);
}
void mostrarDetalles() {
motor.mostrarPotencia();
ruedas.mostrarTamaño();
}
};

// funcion principal 
int main() {
Coche miCoche;
miCoche.setDetalles(150, 16); // Establecemos la potencia del motor y el tamaño de las
ruedas
miCoche.conducir();
miCoche.mostrarDetalles();
return 0;
}
