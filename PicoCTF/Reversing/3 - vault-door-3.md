## Descripción
This vault uses for-loops and byte arrays. The source code for this vault is here: [VaultDoor3.java](https://jupiter.challenges.picoctf.org/static/943ea40e3f54fca6d2145fa7aadc5e09/VaultDoor3.java)
## Pistas 
Make a table that contains each value of the loop variables and the corresponding buffer index that it writes to.
## Solución
para este codigo tomaremos el valor que seria a reorganizar por bloques y  tomamos el contenido del metodo checkpassword, haciendo un codigo nuevo en java nos dara la flag correcta

public class PasswordCheck {
    public static void main(String[] args) {
  
        String password = "jU5t_a_sna_3lpm18g947_u_4_m9r54f";


        char[] buffer = new char[32];
        int i;

        for (i = 0; i < 8; i++) {
            buffer[i] = password.charAt(i);
        }

        for (i = 8; i < 16; i++) {
            buffer[i] = password.charAt(23 - i);
        }

        for (i = 16; i < 32; i += 2) {
            buffer[i] = password.charAt(46 - i);
        }

        for (i = 31; i >= 17; i -= 2) {
            buffer[i] = password.charAt(i);
        }


        String reorganizedPassword = new String(buffer);
        System.out.println("Resultado del buffer reorganizado: " + reorganizedPassword);
    }
}
## Bandera
picoCTF{jU5t_a_s1mpl3_an4gr4m_4_u_79958f}