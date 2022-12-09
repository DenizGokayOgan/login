# login
    import java.util.Scanner;
    public class Main {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        String username;
        String answer;
        int password ;
        int newPassword;

        System.out.print("Username: ");
        username = input.nextLine();
        System.out.print("Password:  ");
        password = input.nextInt();
        input.nextLine();


    if((username.equals("deniz")) && (password == 181818)){
            System.out.println("Succesfully");
        }
    else{
        if (!username.equals("deniz")) {
            System.out.println("Username failed");
        }
            System.out.print("Wrong password. ");
            System.out.println("If you forget password, write yes");
            answer = input.nextLine();
            if(answer.equals("yes")) {
                System.out.println("Enter new password");
                newPassword = input.nextInt();

                if (newPassword != 181818) {
                    System.out.println("New password created");
                }
                else{
                    System.out.println("Please enter different password");
                }
            }
            else{
                System.out.println("Error");
            }
        }



        }
    }




