import javax.swing.*;
import java.awt.event.*;
import java.awt.*;


public class Login extends JFrame implements ActionListener {
    
    JLabel etiquetalog1, etiquetalog2, etiquetalog3;
    JTextField txtusuario;
    JPasswordField txtcontrasena;
    JButton boton1, boton2;
    JPanel panel1;
    Color color1, color2;

    Login(){

        // Si este formulario se ejecuta en otra PC no cargara la imagen de login.
        etiquetalog1 = new JLabel(new ImageIcon("C:\\Users\\gerny\\Desktop\\Programacion-1 (TDS-003)\\Login Aplicacion Recursos\\Logino-1.png")); 
        etiquetalog1.setBounds(20, 20, 400, 80);

        etiquetalog2 = new JLabel("Usuario");
        etiquetalog2.setBounds(195, 100, 80, 20);
        etiquetalog2.setFont(new Font("Helvetica",3,13));

        txtusuario = new JTextField();
        txtusuario.setBounds(150, 120, 135, 22);

        etiquetalog3 = new JLabel("Contraseña");
        etiquetalog3.setBounds(185, 160, 80, 20);
        etiquetalog3.setFont(new Font("Helvetica",3,13));

        txtcontrasena = new JPasswordField();
        txtcontrasena.setBounds(150, 180, 135, 22);

        boton1 = new JButton("Ingresar");
        boton1.setBounds(167, 220, 100, 20);

        boton2 = new JButton("Registrarse");
        boton2.setBounds(162, 260, 110, 20);

        color1 = new Color(204,235,249);
        color2 = new Color(85, 175, 216);

        panel1 = new JPanel();
        panel1.setLayout(null);

        panel1.add(etiquetalog1);
        panel1.add(etiquetalog2);
        panel1.add(etiquetalog3);

        panel1.add(txtusuario);
        panel1.add(txtcontrasena);

        panel1.add(boton1);
       // boton1.setBackground(color2);
        boton1.addActionListener(this);

        panel1.add(boton2);
       // boton2.setBackground(color2);
        boton2.addActionListener(this);

        //setLayout(null);
        setTitle("TDS-003 / Gerny A. Feliz Aquino 2015-3109");
        add(panel1);               // colores:  #CCEBF9   /   204, 235, 249
        //getContentPane().setBackground(new Color(204, 235, 249)); //no me funciona el fondo
        setBounds(440, 150, 450, 400);  //width ancho - height alto
        setResizable(false);
        setVisible(true);
        setDefaultCloseOperation(EXIT_ON_CLOSE);
    }

    //_________________________________________________________________________________________________________________________________________
    public class Principal extends JFrame implements ActionListener{
                
    		public JTable tabla;
            public JLabel usuario, nombre, apellido, telefono, correo, contrasena;
            private JScrollBar scroll;
            private JButton boton1, boton2, boton3, boton4;
        
            Principal(){
        

        
            }
            public void actionPerformed(ActionEvent e){
        
            }
        
        }
//_______________________________________________________________________________________________________________________________________________
        public class Registro extends JFrame implements ActionListener{
            
                public JPanel panel2;
                public JLabel usuario, nombre, apellido, telefono, correo, contrasena;
                private JTextField txtusuario, txtnombre, txtapellido, txttelefono, txtcorreo, txtcontrasena;
                private JButton boton1;
            
                Registro(){
            
                usuario = new JLabel("Usuario: ");
                usuario.setBounds(40,20,100,80);

                nombre = new JLabel("Nombre: ");
                nombre.setBounds(40, 40, 100, 80);

                apellido = new JLabel("Apellido: ");
                apellido.setBounds(40, 60, 100, 80);

                telefono = new JLabel("Telefono: ");
                telefono.setBounds(40, 80, 100, 80);

                correo = new JLabel("Correo: ");
                correo.setBounds(40, 100, 100, 80);

                contrasena = new JLabel("Contraseña: ");
                contrasena.setBounds(40, 120, 100, 80);
//---------------------------------------------------------------------------------------------
                txtusuario = new JTextField();
                txtusuario.setBounds(120, 51, 120, 20);

                txtnombre = new JTextField();
                txtnombre.setBounds(120, 71, 120, 20);

                txtapellido = new JTextField();
                txtapellido.setBounds(120, 91, 120, 20);

                txttelefono = new JTextField();
                txttelefono.setBounds(120, 111, 120, 20);

                txtcorreo = new JTextField();
                txtcorreo.setBounds(120, 131, 120, 20);

                txtcontrasena = new JTextField();
                txtcontrasena.setBounds(120, 151, 120, 20);

                boton1 = new JButton("Confirmar");
                boton1.setBounds(90, 183, 100, 20);
                boton1.addActionListener(this);

                panel2 = new JPanel();
                panel2.setLayout(null);

                panel2.add(usuario);
                panel2.add(txtusuario);
                panel2.add(nombre);
                panel2.add(txtnombre);
                panel2.add(apellido);
                panel2.add(txtapellido);
                panel2.add(telefono);
                panel2.add(txttelefono);
                panel2.add(correo);
                panel2.add(txtcorreo);
                panel2.add(contrasena);
                panel2.add(txtcontrasena);
                panel2.add(boton1);

                setTitle("Registro de Datos");
                add(panel2);
                setSize(300, 300);
                setLocationRelativeTo(null);
                setResizable(false);
                setVisible(true);

                }
                public void actionPerformed(ActionEvent e){
            
                    
                    if(e.getSource() == boton1){
                        setVisible(false);
                        new Login();
                    }
                }
            
            }



    public static void main(String[] args){
        new Login();
        
    }

    public void actionPerformed(ActionEvent e){
        
        if(e.getSource() == boton1){

            String texto = txtusuario.getText().trim();
            
            if(texto.equals("")){
                JOptionPane.showMessageDialog(null,"debe ingresar su usuario y contraseña, si no está registrado debe registrarse");
            } else {
                // LLamar a Principal
                setVisible(false);
                Principal principal = new Principal();
                principal.setTitle("Bienvenido "+texto);
            }
            
        }
        if(e.getSource() == boton2){
            setVisible(false);
            Registro registro = new Registro();
            registro.setTitle("Registro de Datos");
        }
    }

}
