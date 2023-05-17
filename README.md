# examen2
ejercicio 2
public class FrecuenciaCardiaca {
private String nombre;
private String paterno;
private String materno;
private int diadenacimiento;
private int mesnacimiento;
private int añonacimiento;

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public String getPaterno() {
        return paterno;
    }

    public void setPaterno(String paterno) {
        this.paterno = paterno;
    }

    public String getMaterno() {
        return materno;
    }

    public void setMaterno(String materno) {
        this.materno = materno;
    }

    public int getDiadenacimiento() {
        return diadenacimiento;
    }

    public void setDiadenacimiento(int diadenacimiento) {
        this.diadenacimiento = diadenacimiento;
    }

    public int getMesnacimiento() {
        return mesnacimiento;
    }

    public void setMesnacimiento(int mesnacimiento) {
        this.mesnacimiento = mesnacimiento;
    }

    public int getAñonacimiento() {
        return añonacimiento;
    }

    public void setAñonacimiento(int añonacimiento) {
        this.añonacimiento = añonacimiento;
    }

    public String mostraredadpersona(){
        String ed = diadenacimiento+"/"+mesnacimiento+"/"+añonacimiento;
        return ed;
    }
    public int getedad()
    {
        int hoydia= 06;
        int hoymes=05;
        int hoyaño= 2023;
        int calculo1= 1000*hoyaño+100+hoymes+hoydia;
        int calculo2= 1000*añonacimiento+100*mesnacimiento+diadenacimiento;
        
        return(int)(calculo1-calculo2)/1000;
    }
    public int getfrecuenciacardiacamaxima()
    {
        return 220- getedad();
    }
    public String getintervalofrecuencialcardiacaesperada()
    {
     return String.format("[%,1f - %,1f]",
     (float )getfrecuenciacardiacamaxima() *0.58,
     (float) getfrecuenciacardiacamaxima()* 0.58);    }
        
    }
    
