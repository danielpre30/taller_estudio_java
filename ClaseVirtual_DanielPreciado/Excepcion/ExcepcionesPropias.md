# Excepciones Propias
Para crear y lanzar una excepción propia tenemos que definir la clase ExcepcionPropia derivada de la clase base Exception.

    public class ExcepcionPropia extends Exception {
        public ExcepcionPropia(String msg) {
            super(msg);
        }
    }

## El método que puede lanzar una excepción
La función miembro que lanza una excepción tiene la declaración habitual que cualquier otro método pero se le añade a continuación la palabra reservada *throws* seguido de la excepción o excepciones que puede lanzar.
    
    static void rango(int num, int den)throws ExcepcionIntervalo{
        if((num>100)||(den<-5)){
            throw new ExcepcionIntervalo("Números fuera del intervalo");
        }
    }