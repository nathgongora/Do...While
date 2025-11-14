# Do...While
Algoritmo que peça para o usuário digitar vários números e calcule a média desses números. O algoritmo deve parar quando o usuário digitar zero.

public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        int valor = 0;
        double soma = 0.0;
        double media = 0.0;
        int cont = 0;
        
        do { 
            System.out.println("Digite um valor para media");
            valor = sc.nextInt();
            soma += valor;
            cont ++;
        } while (valor > 0);
         
        soma += valor;
        
        if (cont > 1) {
            media = soma/(cont-1);
        }
        
        System.out.println("Resultado e: " + media);
    }
}
