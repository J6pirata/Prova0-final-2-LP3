# Prova0-final-2-LP3
Segunda prova final de Liguagem de programação 3°semestre


import java.util.Scanner;

public class ConsultaAgendada {

    Scanner Ler = new Scanner(system.in);

    private int Data;
    private int Hora;
    static int quantidade;
    private string nomePaciente;
    private string nomeMedico;

    public ConsultaAgendada() {
        System.out.print("Digite a data:");
        this.Data = Ler.nextInt();
        System.out.print("Digite a hora:");
        this.Hora = Ler.nextInt();
        System.out.print("Digite o nome do paciente:");
        this.nomePaciente = Ler.nextLine();
        System.out.print("Digite a nome do medico:");
        this.nomeMedico = Ler.nextLine();
        quantidade++;
    }

    public ConsultaAgendada(int h, int mi, int s, int d, int m, int a, string p, string m2) {
        this.Hora = h;
        this.Hora = mi;
        this.Hora = s;
        this.Data = d;
        this.Data = m;
        this.Data = a;
        this.nomePaciente = p;
        this.nomeMedico = m2;
        quantidade++;

    void Verdados() {
        System.out.print(this.h + ":" + this.mi + ":" + this.s);
        System.out.print(this.d + "/" + this.m + "/" + this.a);
        System.out.print(this.p + "paciente e " + this.m2 + "médico");
    }

    }

    public ConsultaAgendada(Data d, Hora h, String p, String m) {
       d =  this.setData() ;
       h=   this.setHora();
       p =  this.setnomePaciente() ;
       m = this.setnomeMedico() ;
        quantidade++;

    void Verdados2() {
        system.out.print(this.d + "-" + this.h + "-" + this.p + "-" + this.m);
    }

    }

    public void setData(int a, int b, int c) {
        this.Data = a;
        this.Data = b;
        this.Data = c;

    }

    public void setData() {
        System.out.print("Digite o dia ");
        this.Data = Ler.nextInt();
        System.out.print("Digite o mês ");
        this.Data = Ler.nextInt();
        System.out.print("Digite o ano ");
        this.Data = Ler.nextInt();

    }

    public setHora(int a, int b, int c){
        this.Hora = a;
        this.Hora = b;
        this.Hora = c;

    }

    public setHora(){
        System.out.print("Digite o Hora ");
        this.Hora = Ler.nextInt();
        System.out.print("Digite o minuto ");
        this.Hora = Ler.nextInt();
        System.out.print("Digite o segundo ");
        this.Hora = Ler.nextInt();

    }

    public  setnomePaciente(String p) {
             this.nomePaciente= p;
    }

    public  setnomePaciente() {
        System.out.print("digite novamente nome do paciente");
        this.nomePaciente = Ler.nextLine();
    }

    public setnomeMedico(String m){
        this.nomeMedico = m;
    }

    public setnomeMedico(){
        System.out.print("Digite novamente o nome do medico");
        this.nomeMedico = Ler.nextLine();
    }

    public String getnomePaciente() {
        return this.nomePaciente;
    }

    public String getnomeMedico() {
        return this.nomeMedico;
    }

    public int getAmostra() {
        system.out.print("Quantida dconsulta marcada :", quantidade);
    }

public class Programa {
    public static void main(String [] args) {

        ConsultaAgendada p1 = new ConsultaAgendada();
        p1.Verdados();

        ConsultaAgendada p2 = new ConsultaAgendada();
        p2.Verdados2();
        p2.getAmostra();

    }
}
