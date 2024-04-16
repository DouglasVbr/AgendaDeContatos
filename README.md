package AgendaDeContatos;

import javax.swing.JOptionPane;
import javax.swing.JTextField;

public class AgendaContatosUI extends javax.swing.JFrame {

    private Agenda agenda;

    public AgendaContatosUI() {
        super("Agenda de Contatos");
        agenda = new Agenda(100); // Criando uma agenda com tamanho máximo de 100 contatos
        initComponents();
    }
    
    /*@Test*/
    public void testLimparCampos() {
        AgendaContatosUI instance = new AgendaContatosUI();
        
        // Configurar os campos com algum texto
        instance.txtNome.setText("João");
        instance.txtFone.setText("123456789");
        instance.txtEmail.setText("joao@example.com");
        
        // Chamar o método para limpar os campos
        instance.limparCampos();
        
        // Verificar se os campos foram limpos corretamente
        assertEquals("", instance.txtNome.getText());
        assertEquals("", instance.txtFone.getText());
        assertEquals("", instance.txtEmail.getText());
    }

    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        jPanel1 = new javax.swing.JPanel();
        btnExcluir = new javax.swing.JButton();
        lblTitulo = new javax.swing.JLabel();
        lblNome = new javax.swing.JLabel();
        lblFone = new javax.swing.JLabel();
        lblEmail = new javax.swing.JLabel();
        txtNome = new javax.swing.JTextField();
        txtFone = new javax.swing.JTextField();
        txtEmail = new javax.swing.JTextField();
        btnPesquisar = new javax.swing.JButton();
        btnSalvar = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        btnExcluir.setText("EXCLUIR");
        btnExcluir.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btnExcluirActionPerformed(evt);
            }
        });

        lblTitulo.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        lblTitulo.setText("AGENDA DE CONTATOS");

        lblNome.setFont(new java.awt.Font("Tahoma", 1, 12)); // NOI18N
        lblNome.setText("NOME:");

        lblFone.setFont(new java.awt.Font("Tahoma", 1, 12)); // NOI18N
        lblFone.setText("FONE:");

        lblEmail.setFont(new java.awt.Font("Tahoma", 1, 12)); // NOI18N
        lblEmail.setText("E-MAIL:");

        txtNome.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                txtNomeActionPerformed(evt);
            }
        });

        txtFone.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                txtFoneActionPerformed(evt);
            }
        });

        txtEmail.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                txtEmailActionPerformed(evt);
            }
        });

        btnPesquisar.setText("PESQUISAR");
        btnPesquisar.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btnPesquisarActionPerformed(evt);
            }
        });

        btnSalvar.setText("SALVAR");
        btnSalvar.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                btnSalvarActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout jPanel1Layout = new javax.swing.GroupLayout(jPanel1);
        jPanel1.setLayout(jPanel1Layout);
        jPanel1Layout.setHorizontalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(jPanel1Layout.createSequentialGroup()
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(jPanel1Layout.createSequentialGroup()
                        .addGap(59, 59, 59)
                        .addComponent(btnSalvar)
                        .addGap(27, 27, 27)
                        .addComponent(btnPesquisar)
                        .addGap(28, 28, 28)
                        .addComponent(btnExcluir))
                    .addGroup(jPanel1Layout.createSequentialGroup()
                        .addGap(43, 43, 43)
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                            .addComponent(lblEmail)
                            .addComponent(lblFone)
                            .addComponent(lblNome))
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                            .addComponent(txtEmail)
                            .addComponent(txtFone)
                            .addComponent(txtNome, javax.swing.GroupLayout.PREFERRED_SIZE, 238, javax.swing.GroupLayout.PREFERRED_SIZE))))
                .addGap(0, 77, Short.MAX_VALUE))
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                .addComponent(lblTitulo)
                .addGap(126, 126, 126))
        );
        jPanel1Layout.setVerticalGroup(
            jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(javax.swing.GroupLayout.Alignment.TRAILING, jPanel1Layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(lblTitulo)
                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED, 32, Short.MAX_VALUE)
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(lblNome)
                    .addComponent(txtNome, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(18, 18, 18)
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(lblFone)
                    .addComponent(txtFone, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(25, 25, 25)
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                    .addComponent(lblEmail)
                    .addComponent(txtEmail, javax.swing.GroupLayout.PREFERRED_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(58, 58, 58)
                .addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(btnSalvar)
                    .addComponent(btnPesquisar)
                    .addComponent(btnExcluir))
                .addGap(51, 51, 51))
        );

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
        );

        pack();
        setLocationRelativeTo(null);
    }// </editor-fold>                        

    private void btnExcluirActionPerformed(java.awt.event.ActionEvent evt) {                                           
        String nome = txtNome.getText();
        agenda.excluirContato(nome);
        limparCampos();
    }                                          

    private void btnSalvarActionPerformed(java.awt.event.ActionEvent evt) {                                          
       String nome = txtNome.getText();
    String telefone = txtFone.getText();
    String email = txtEmail.getText(); 
    Contato contato = new Contato(nome, telefone, email); // Atualizando para passar o email
    agenda.adicionarContato(contato);
    
    limparCampos();
    }                                         

    private void btnPesquisarActionPerformed(java.awt.event.ActionEvent evt) {                                             
        String nome = txtNome.getText();
        Contato contato = agenda.pesquisarContato(nome);
        if (contato != null) {
            JOptionPane.showMessageDialog(null, "Contato encontrado:\n" + contato.toString());
        } else {
            JOptionPane.showMessageDialog(null, "Contato não encontrado!");
        }
    }                                            

    private void txtNomeActionPerformed(java.awt.event.ActionEvent evt) {                                        

    }                                       

    private void txtFoneActionPerformed(java.awt.event.ActionEvent evt) {                                        

    }                                       

    private void txtEmailActionPerformed(java.awt.event.ActionEvent evt) {                                         

    }                                        

    void limparCampos() {
        txtNome.setText("");
        txtFone.setText("");
        txtEmail.setText("");
    }

    public static void main(String args[]) {
        /* Set the Nimbus look and feel */
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code (optional) ">
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
         * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
         */
        try {
            for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
                if ("Nimbus".equals(info.getName())) {
                    javax.swing.UIManager.setLookAndFeel(info.getClassName());
                    break;
                }
            }
        } catch (ClassNotFoundException ex) {
            java.util.logging.Logger.getLogger(AgendaContatosUI.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(AgendaContatosUI.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(AgendaContatosUI.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(AgendaContatosUI.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new AgendaContatosUI().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton btnExcluir;
    private javax.swing.JButton btnPesquisar;
    private javax.swing.JButton btnSalvar;
    private javax.swing.JPanel jPanel1;
    private javax.swing.JLabel lblEmail;
    private javax.swing.JLabel lblFone;
    private javax.swing.JLabel lblNome;
    private javax.swing.JLabel lblTitulo;
    private javax.swing.JTextField txtEmail;
    private javax.swing.JTextField txtFone;
    private javax.swing.JTextField txtNome;
    // End of variables declaration                   

    private void assertEquals(String string, String text) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

    void setNome(String joão) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

    void setEmail(String joaoexamplecom) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

}


package AgendaDeContatos;


public class Contato {

   
    private String nome;
    private String telefone;
    private String email;

    public Contato(String nome, String telefone, String email) {
        this.nome = nome;
        this.telefone = telefone;
        this.email = email;
    }

    Contato(String nome, String telefone) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

    // Getters e setters
    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public String getTelefone() {
        return telefone;
    }

    public void setTelefone(String telefone) {
        this.telefone = telefone;
    }

    public String getEmail() {
        return email;
    }

    public void setEmail(String email) {
        this.email = email;
    }

    @Override
    public String toString() {
        return "Nome: " + nome + "\nTelefone: " + telefone + "\nE-mail: " + email;
    }
    
    
}
   

package AgendaDeContatos;

import javax.swing.JOptionPane;

public class Agenda {
    private Contato[] contatos;
    private int tamanhoMaximo;
    private int quantidadeContatos;

    public Agenda(int tamanhoMaximo) {
        this.tamanhoMaximo = tamanhoMaximo;
        contatos = new Contato[tamanhoMaximo];
        quantidadeContatos = 0;
    }

    // Método para adicionar um contato à agenda
    public void adicionarContato(Contato contato) {
        if (quantidadeContatos < tamanhoMaximo) {
            contatos[quantidadeContatos++] = contato;
            JOptionPane.showMessageDialog(null, "Contato adicionado com sucesso!");
        } else {
            JOptionPane.showMessageDialog(null, "Agenda cheia! Não é possível adicionar mais contatos.");
        }
    }

    // Método para pesquisar um contato na agenda pelo nome
    public Contato pesquisarContato(String nome) {
        for (int i = 0; i < quantidadeContatos; i++) {
            if (contatos[i].getNome().equalsIgnoreCase(nome)) {
                return contatos[i];
            }
        }
        return null; // Retornar null se o contato não for encontrado
    }

    // Método para excluir um contato da agenda pelo nome
    public void excluirContato(String nome) {
        for (int i = 0; i < quantidadeContatos; i++) {
            if (contatos[i].getNome().equalsIgnoreCase(nome)) {
                // Desloca os contatos à direita para preencher a posição removida
                for (int j = i; j < quantidadeContatos - 1; j++) {
                    contatos[j] = contatos[j + 1];
                }
                quantidadeContatos--;
                JOptionPane.showMessageDialog(null, "Contato excluído com sucesso!");
                return; // Não precisa continuar o loop após encontrar e excluir o contato
            }
        }
        JOptionPane.showMessageDialog(null, "Contato não encontrado!");
    }

    // Método para obter o total de contatos na agenda
    public int getTotalContatos() {
        return quantidadeContatos;
    }

    void excluirContato(Contato contato) {
        throw new UnsupportedOperationException("Not supported yet."); //To change body of generated methods, choose Tools | Templates.
    }

   
}
  

package AgendaDeContatos;

import org.junit.After;
import org.junit.AfterClass;
import org.junit.Before;
import org.junit.BeforeClass;
import org.junit.Test;
import static org.junit.Assert.*;


public class AgendaContatosUITest {
    
    public AgendaContatosUITest() {
    }
    
    @BeforeClass
    public static void setUpClass() {
    }
    
    @AfterClass
    public static void tearDownClass() {
    }
    
    @Before
    public void setUp() {
    }
    
    @After
    public void tearDown() {
    }

    /**
     * Test of testLimparCampos method, of class AgendaContatosUI.
     */
    @Test
    public void testTestLimparCampos() {
       // Crie uma instância da AgendaContatosUI
        AgendaContatosUI agendaUI = new AgendaContatosUI();
        
        // Defina o estado inicial, por exemplo, preencha alguns campos
        agendaUI.setName("João");
        agendaUI.setTitle("joao@example.com");
        
        // Chame o método a ser testado
        agendaUI.limparCampos();
        
        // Verifique se os campos foram limpos corretamente
        assertEquals("", agendaUI.getName());
        assertEquals("", agendaUI.getExtendedState());
    }

    /**
     * Test of main method, of class AgendaContatosUI.
     */
    @Test
    public void testMain() {
       
    }

    /**
     * Test of limparCampos method, of class AgendaContatosUI.
     */
    @Test
    public void testLimparCampos() {
        System.out.println("limparCampos");
        AgendaContatosUI instance = new AgendaContatosUI();
        instance.limparCampos();
        // TODO review the generated test code and remove the default call to fail.
        fail("The test case is a prototype.");
    }

    /**
     * Test of setNome method, of class AgendaContatosUI.
     */
    @Test
    public void testSetNome() {
        System.out.println("setNome");
        String joão = "";
        AgendaContatosUI instance = new AgendaContatosUI();
        instance.setNome(joão);
        // TODO review the generated test code and remove the default call to fail.
        fail("The test case is a prototype.");
    }

    /**
     * Test of setEmail method, of class AgendaContatosUI.
     */
    @Test
    public void testSetEmail() {
        System.out.println("setEmail");
        String joaoexamplecom = "";
        AgendaContatosUI instance = new AgendaContatosUI();
        instance.setEmail(joaoexamplecom);
        // TODO review the generated test code and remove the default call to fail.
        fail("The test case is a prototype.");
    }
    
}



package AgendaDeContatos;

import org.junit.After;
import org.junit.AfterClass;
import org.junit.Before;
import org.junit.BeforeClass;
import org.junit.Test;
import static org.junit.Assert.*;
import static org.junit.Assert.assertEquals;
import static org.junit.Assert.assertNotNull;
/**
 *
 * @author Douglas
 */
public class AgendaTest {
    
    public AgendaTest() {
    }
    
    @BeforeClass
    public static void setUpClass() {
    }
    
    @AfterClass
    public static void tearDownClass() {
    }
    
    @Before
    public void setUp() {
    }
    
    @After
    public void tearDown() {
    }

    /**
     * Test of adicionarContato method, of class Agenda.
     */
    @Test
    public void testAdicionarContato() {
        Agenda agenda = new Agenda(0);
        
        // Adicione um contato
        Contato contato = new Contato("João", "123456789");
        agenda.adicionarContato(contato);
        
        // Verifique se o contato foi adicionado corretamente
        assertEquals(1, agenda.getTotalContatos());
    }

    @Test
    public void testPesquisarContato() {
        Agenda agenda = new Agenda(0);
        
        // Adicione um contato
        Contato contato = new Contato("Maria", "987654321");
        agenda.adicionarContato(contato);
        
        // Pesquise o contato
        Contato contatoEncontrado = agenda.pesquisarContato("Maria");
        
        // Verifique se o contato foi encontrado corretamente
        assertNotNull(contatoEncontrado);
        assertEquals("Maria", contatoEncontrado.getNome());
        assertEquals("987654321", contatoEncontrado.getTelefone());
    }

    @Test
    public void testExcluirContato() {
        Agenda agenda = new Agenda(0);
        
        // Adicione um contato
        Contato contato = new Contato("Carlos", "111222333");
        agenda.adicionarContato(contato);
        
        // Exclua o contato
        agenda.excluirContato("");
        
        // Verifique se o contato foi excluído corretamente
        assertEquals(0, agenda.getTotalContatos());
    }
}
    


package AgendaDeContatos;

import org.junit.After;
import org.junit.AfterClass;
import org.junit.Before;
import org.junit.BeforeClass;
import org.junit.Test;
import static org.junit.Assert.*;

/**
 *
 * @author Douglas
 */
public class ContatoTest {
    
    public ContatoTest() {
    }
    
    @BeforeClass
    public static void setUpClass() {
    }
    
    @AfterClass
    public static void tearDownClass() {
    }
    
    @Before
    public void setUp() {
    }
    
    @After
    public void tearDown() {
    }

    /**
     * Test of getNome method, of class Contato.
     */
    @Test
    public void testGetNome() {
        Contato contato = new Contato("João", "123456789", "joao@example.com");
        assertEquals("João", contato.getNome());
    }

    /**
     * Test of setNome method, of class Contato.
     */
    @Test
    public void testSetNome() {
        Contato contato = new Contato("Maria", "987654321", "maria@example.com");
        contato.setNome("Ana");
        assertEquals("Ana", contato.getNome());
    }

    /**
     * Test of getTelefone method, of class Contato.
     */
    @Test
    public void testGetTelefone() {
        Contato contato = new Contato("Carlos", "111222333", "carlos@example.com");
        assertEquals("111222333", contato.getTelefone());
    }

    /**
     * Test of setTelefone method, of class Contato.
     */
    @Test
    public void testSetTelefone() {
        Contato contato = new Contato("Pedro", "444555666", "pedro@example.com");
        contato.setTelefone("777888999");
        assertEquals("777888999", contato.getTelefone());
    }

    /**
     * Test of getEmail method, of class Contato.
     */
    @Test
    public void testGetEmail() {
        Contato contato = new Contato("Ana", "999888777", "ana@example.com");
        assertEquals("ana@example.com", contato.getEmail());
    }

    /**
     * Test of setEmail method, of class Contato.
     */
    @Test
    public void testSetEmail() {
        Contato contato = new Contato("Mariana", "555444333", "mariana@example.com");
        contato.setEmail("mariana.updated@example.com");
        assertEquals("mariana.updated@example.com", contato.getEmail());
    }

    /**
     * Test of toString method, of class Contato.
     */
    @Test
    public void testToString() {
        Contato contato = new Contato("Lucas", "222333444", "lucas@example.com");
        String expected = "Nome: Lucas, Telefone: 222333444, Email: lucas@example.com";
        assertEquals(expected, contato.toString());
    }
    
}


