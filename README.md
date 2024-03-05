# Livro


PARTE.1 

package livro;

public class LivroOutro {

    private String titulo;
    private String autor;
    private int anoPublicacao;
    private String genero;

    // metodo construtor
    public LivroOutro(String titulo, String autor, int anoPublicacao, String genero) {
        this.titulo = "Dom Casmurro";
        this.autor = "Machado de Assis";
        this.anoPublicacao = 1899;
        this.genero = "Romance";

    }
    
    // metodo acessores
    public String settitulo(String titulo){
        this.titulo = titulo;
        return titulo;
    
    }
    public String gettitulo() {
        return titulo;
    }
    
    public String setautor(String autor){
        this.autor = autor;
        return autor;
    
    }
    public String getautor() {
        return autor;
    }
    
    public int setanoPublicacao(int anoPublicacao){
        this.anoPublicacao = anoPublicacao;
        return anoPublicacao;
    
    }
    public int getanoPublicacao() {
        return anoPublicacao;
    }
    
    public String getgenero() {
        return genero;
    }
    
    public String setgenero(String genero){
        this.genero = genero;
        return genero;
    
    }
    
    public void exibir(){
    
    System.out.println("titulo: " + gettitulo());
        System.out.println("autor: " + getautor());
        System.out.println("ano: " + getanoPublicacao());
        System.out.println("genero: " + getgenero());
    }
    
    // Método para verificar se o livro pertence a um determinado gênero
    
    public boolean pertenceAoGenero(String genero) {
        return this.genero.equalsIgnoreCase(genero);
    }
    

}
PARTE.2

package livro;


public class Livro {

    
    public static void main(String[] args) {
       LivroOutro l1 = new LivroOutro("Dom Casmurro", "Machado de Assis", 1899, "Romance");
       l1.exibir();
       
       
       
       
    }
    
}
