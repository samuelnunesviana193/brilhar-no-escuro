// Projeto: o sirva precisa de luz

int pinoLed = 6; //Define o nome da porta 6 como "pinoLed"
int valorLuz = 0; //Define a variável "valorLuz" como zero

void setup()
{
  pinMode (pinoLed, OUTPUT); //Define a porta 6 como de saída
}

void loop()
{
  valorLuz = analogRead (A0); //Faz a leitura da porta A0 e armazena em "valorLuz"
  if (valorLuz < 80) {        //Condição, se o valorLuz for menor do que 80 unidades
  analogWrite (pinoLed, 255); //Manter o pinoLed desligado (zero)
  }
  else { //Senão
    digitalWrite (pinoLed, LOW); //Ligar o Led, mas com a tensão variando conforme a 
    } 
}
