# Livro


PARTE.1 

// Arquivo: Livro.java
package biblioteca;

public class Livro {
    private String titulo;
    private String autor;
    private int anoPublicacao;
    private String genero;
    
    // Construtor
    public Livro(String titulo, String autor, int anoPublicacao, String genero) {
        this.titulo = "Dom Casmurro";
        this.autor = "Machado de Assis";
        this.anoPublicacao = 1899;
        this.genero = "Romance";
    }
    
    // Métodos acessores
    public String getTitulo() {
        return titulo;
    }
    
    public String getAutor() {
        return autor;
    }
    
    public int getAnoPublicacao() {
        return anoPublicacao;
    }
    
    // Método para verificar se o livro pertence a um determinado gênero
    public boolean pertenceAoGenero(String genero) {
        return this.genero.equalsIgnoreCase(genero);
    }
}

PARTE.2

// Arquivo: Main.java
package biblioteca;

public class Main {
    public static void main(String[] args) {
        // Criando um objeto Livro
        Livro livro1 = new Livro("Dom Casmurro", "Machado de Assis", 1899, "Romance");
        
        // Exibindo informações do livro
        System.out.println("Título: " + livro1.getTitulo());
        System.out.println("Autor: " + livro1.getAutor());
        System.out.println("Ano de Publicação: " + livro1.getAnoPublicacao());
        
        // Verificando se o livro pertence ao gênero "Romance"
        String generoBuscado = "Romance";
        if (livro1.pertenceAoGenero(generoBuscado)) {
            System.out.println("O livro pertence ao gênero '" + generoBuscado + "'.");
        } else {
            System.out.println("O livro não pertence ao gênero '" + generoBuscado + "'.");
        }
    }
}
