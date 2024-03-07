# Livro


PARTE.1 

package livro;


public class Livro {

   
    public static void main(String[] args) {
        // Criando um objeto
        Livro2 Livro2 = new Livro2("Harry Potter e a Pedra Filosofal", "J. K. Rowling", 1997, " Romance, Literatura infantil, Literatura fantástica, Alta fantasia");
        
        // Exibindo informações do livro
        Livro2.exibir();
    }
    
}



PARTE.2

package livro;

public class Livro2 {
    // variaveis
    private String Titulo;
    private String Autor;
    private int AnoPublicacao;
    private String Genero;
    
    // metodo construtor
    public Livro2(String Titulo, String Autor, int AnoPublicacao, String Genero){
        this.Titulo = Titulo;
        this.Autor = Autor;
        this.AnoPublicacao = AnoPublicacao;
        this.Genero = Genero;
    }
    
    // metodo set titulo
    public void setTitulo(String Titulo){
        this.Titulo = Titulo;
    }
    
    // metodo get titulo
    public String getTitulo(){
        return Titulo;
    }
    
    // metodo set autor 
    public void setAutor(String Autor){
        this.Autor = Autor;
    }
    
    // metodo get autor
    public String getAutor(){
        return Autor;
    }
    
    // metodo get anopublicação
    public int getAnoPublicacao(){
        return AnoPublicacao;
    }
    
    // metodo set anopublicação
    public void setAnoPublicacao(int AnoPublicacao){
        this.AnoPublicacao = AnoPublicacao;
    }
    
    // metodo get genero
    public String getGenero(){
        return Genero;
    }
    
    // metodo set genero
    public void setGenero(String Genero){
        this.Genero = Genero;
    }
    
    // metodo para verificar se o livro pertence a um determinado gênero
    public boolean pertenceGenero(String Genero) {
        return this.Genero.equalsIgnoreCase(Genero);
    }
    
    // exibir na tela
    public void exibir(){
        System.out.println("titulo: " + getTitulo());
        System.out.println("autor: " + getAutor ());
        System.out.println("ano de publicação: " + getAnoPublicacao ());
        System.out.println("genero: " + getGenero ());
    }
}

