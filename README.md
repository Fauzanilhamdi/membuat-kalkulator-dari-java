# membuat-kalkulator-dari-java
project ini membuat kalkulator dari java dan koneksi ke dataabse


import java.sql.Connection;
import java.sql.DriverManager;
import javax.swing.JOptionPane;

public class koneksikalkulator extends javax.swing.JFrame { 
    double angkapertama;
    double angkakedua;
    double result;
    String operations;
            
    private Connection fauzan;
    public koneksikalkulator() {
        initComponents();
    }
     private void koneksikalkulator(){
         try{
            Class.forName("com.mysql.jdbc.Driver");
        fauzan = DriverManager.getConnection("jdbc:mysql://localhost:3306/db_kalkulatorjava","root","");
             JOptionPane.showMessageDialog(null, "koneksi ke databases");                    
         } catch (Exception e) {   
             System.out.println("seperti nya ada yang eror"+ e.getMessage());
         }
     }
    
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        jtxtDisplay = new javax.swing.JTextField();
        jBtn1 = new javax.swing.JButton();
        jBtn2 = new javax.swing.JButton();
        jBtn3 = new javax.swing.JButton();
        jBtn4 = new javax.swing.JButton();
        jBtn9 = new javax.swing.JButton();
        jBtn6 = new javax.swing.JButton();
        jBtn7 = new javax.swing.JButton();
        jBtn8 = new javax.swing.JButton();
        jBtn10 = new javax.swing.JButton();
        jBtn13 = new javax.swing.JButton();
        jBtn11 = new javax.swing.JButton();
        jBtn12 = new javax.swing.JButton();
        jBtn5 = new javax.swing.JButton();
        jBtn14 = new javax.swing.JButton();
        jBtn15 = new javax.swing.JButton();
        jBtn16 = new javax.swing.JButton();
        jBtn17 = new javax.swing.JButton();
        jBtn18 = new javax.swing.JButton();

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setBackground(new java.awt.Color(0, 0, 0));

        jtxtDisplay.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jtxtDisplay.setHorizontalAlignment(javax.swing.JTextField.RIGHT);

        jBtn1.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn1.setText("1");
        jBtn1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn1ActionPerformed(evt);
            }
        });

        jBtn2.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn2.setText("2");
        jBtn2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn2ActionPerformed(evt);
            }
        });

        jBtn3.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn3.setText("3");
        jBtn3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn3ActionPerformed(evt);
            }
        });

        jBtn4.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn4.setText("4");
        jBtn4.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn4ActionPerformed(evt);
            }
        });

        jBtn9.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn9.setText("9");
        jBtn9.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn9ActionPerformed(evt);
            }
        });

        jBtn6.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn6.setText("6");
        jBtn6.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn6ActionPerformed(evt);
            }
        });

        jBtn7.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn7.setText("7");
        jBtn7.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn7ActionPerformed(evt);
            }
        });

        jBtn8.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn8.setText("8");
        jBtn8.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn8ActionPerformed(evt);
            }
        });

        jBtn10.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn10.setText("0");
        jBtn10.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn10ActionPerformed(evt);
            }
        });

        jBtn13.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn13.setText("/");
        jBtn13.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn13ActionPerformed(evt);
            }
        });

        jBtn11.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn11.setText("+");
        jBtn11.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn11ActionPerformed(evt);
            }
        });

        jBtn12.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn12.setText("-");
        jBtn12.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn12ActionPerformed(evt);
            }
        });

        jBtn5.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn5.setText("5");
        jBtn5.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn5ActionPerformed(evt);
            }
        });

        jBtn14.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn14.setText("*");
        jBtn14.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn14ActionPerformed(evt);
            }
        });

        jBtn15.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn15.setText("+/-");
        jBtn15.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn15ActionPerformed(evt);
            }
        });

        jBtn16.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn16.setText(".");
        jBtn16.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn16ActionPerformed(evt);
            }
        });

        jBtn17.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn17.setText("C");
        jBtn17.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn17ActionPerformed(evt);
            }
        });

        jBtn18.setFont(new java.awt.Font("Tahoma", 1, 18)); // NOI18N
        jBtn18.setText("=");
        jBtn18.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                jBtn18ActionPerformed(evt);
            }
        });

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addContainerGap()
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(jBtn9, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(jBtn10, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                        .addComponent(jBtn11, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(jBtn12, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addGroup(layout.createSequentialGroup()
                        .addComponent(jBtn5, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                        .addComponent(jBtn6, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                        .addComponent(jBtn7, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGap(10, 10, 10)
                        .addComponent(jBtn8, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE))
                    .addGroup(layout.createSequentialGroup()
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING, false)
                            .addComponent(jBtn17, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                            .addGroup(layout.createSequentialGroup()
                                .addComponent(jBtn13, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                                .addGap(10, 10, 10)
                                .addComponent(jBtn14, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)))
                        .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                            .addGroup(layout.createSequentialGroup()
                                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                                .addComponent(jBtn18, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
                            .addGroup(layout.createSequentialGroup()
                                .addGap(6, 6, 6)
                                .addComponent(jBtn15)
                                .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)
                                .addComponent(jBtn16, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE))))
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING, false)
                        .addComponent(jtxtDisplay, javax.swing.GroupLayout.Alignment.LEADING)
                        .addGroup(javax.swing.GroupLayout.Alignment.LEADING, layout.createSequentialGroup()
                            .addComponent(jBtn1, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                            .addComponent(jBtn2, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn3, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
                            .addComponent(jBtn4, javax.swing.GroupLayout.PREFERRED_SIZE, 64, javax.swing.GroupLayout.PREFERRED_SIZE))))
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGroup(layout.createSequentialGroup()
                .addContainerGap()
                .addComponent(jtxtDisplay, javax.swing.GroupLayout.PREFERRED_SIZE, 47, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGap(18, 18, 18)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn1, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn2, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn3, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn4, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(18, 18, 18)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn5, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn6, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn7, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn8, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(18, 18, 18)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn9, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn10, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn11, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn12, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(18, 18, 18)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn14, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn15, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn16, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn13, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addGap(18, 18, 18)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn18, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn17, javax.swing.GroupLayout.PREFERRED_SIZE, 61, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addContainerGap(21, Short.MAX_VALUE))
        );

        pack();
    }// </editor-fold>                        

    private void jBtn2ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn2.getText();
        jtxtDisplay.setText(Enternumber);   
    }                                     

    private void jBtn4ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        String Enternumber = jtxtDisplay.getText() + jBtn4.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn17ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        jtxtDisplay.setText("");
    }                                      

    private void jBtn18ActionPerformed(java.awt.event.ActionEvent evt) {                                       
       
        String answer;
        angkakedua = Double.parseDouble(jtxtDisplay.getText());
        if (operations == "+")
        {
            result = angkapertama + angkakedua;
            answer = String.format("%.0f",result);
            jtxtDisplay.setText(answer);
        }
        else if (operations == "-")
        {
            result = angkapertama - angkakedua;
            answer = String.format("%.0f",result);
            jtxtDisplay.setText(answer);
            
        }
        else if (operations == "*")
        {
            result = angkapertama * angkakedua;
            answer = String.format("%.0f",result);
            jtxtDisplay.setText(answer);
            
        }
        else if (operations == "/")
        {
            result = angkapertama / angkakedua;
            answer = String.format("%.0f",result);
            jtxtDisplay.setText(answer);
            
        }
        
        else if(operations == "%")
        {
            result = angkapertama % angkakedua;
            answer = String.format("%.0f",result);
            jtxtDisplay.setText(answer);
            
        }
    }                                      

    private void jBtn1ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn1.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn3ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn3.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn6ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn6.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn7ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn7.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn8ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn8.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn9ActionPerformed(java.awt.event.ActionEvent evt) {                                      
        
        String Enternumber = jtxtDisplay.getText() + jBtn9.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn10ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        
        String Enternumber = jtxtDisplay.getText() + jBtn10.getText();
        jtxtDisplay.setText(Enternumber);
        
    }                                      

    private void jBtn5ActionPerformed(java.awt.event.ActionEvent evt) {                                      

        String Enternumber = jtxtDisplay.getText() + jBtn5.getText();
        jtxtDisplay.setText(Enternumber);
    }                                     

    private void jBtn11ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        
        angkapertama = Double.parseDouble(jtxtDisplay.getText());
        jtxtDisplay.setText("");
        operations = "+";
    }                                      

    private void jBtn12ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        
        angkapertama = Double.parseDouble(jtxtDisplay.getText());
        jtxtDisplay.setText("");
        operations = "-";
    }                                      

    private void jBtn13ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        angkapertama = Double.parseDouble(jtxtDisplay.getText());
        jtxtDisplay.setText("");
        operations = "/";
    }                                      

    private void jBtn14ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        angkapertama = Double.parseDouble(jtxtDisplay.getText());
        jtxtDisplay.setText("");
        operations = "*";
    }                                      

    private void jBtn15ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        
        double ops = Double.parseDouble(String.valueOf(jtxtDisplay.getText()));
        ops = ops * (-1);
        jtxtDisplay.setText(String.valueOf(ops));
    }                                      

    private void jBtn16ActionPerformed(java.awt.event.ActionEvent evt) {                                       
        // TODO add your handling code here:
    }                                      

    /**
     * @param args the command line arguments
     */
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
            java.util.logging.Logger.getLogger(koneksikalkulator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (InstantiationException ex) {
            java.util.logging.Logger.getLogger(koneksikalkulator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (IllegalAccessException ex) {
            java.util.logging.Logger.getLogger(koneksikalkulator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        } catch (javax.swing.UnsupportedLookAndFeelException ex) {
            java.util.logging.Logger.getLogger(koneksikalkulator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
        }
        //</editor-fold>

        /* Create and display the form */
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new koneksikalkulator().setVisible(true);
                try {
                 JOptionPane.showMessageDialog(null, "koneksi ke database sukses");   
                } catch (Exception e) {
                    System.out.println("seperti nya ada yang eror"+ e.getMessage());
                }
            }
        });
    }

    // Variables declaration - do not modify                     
    private javax.swing.JButton jBtn1;
    private javax.swing.JButton jBtn10;
    private javax.swing.JButton jBtn11;
    private javax.swing.JButton jBtn12;
    private javax.swing.JButton jBtn13;
    private javax.swing.JButton jBtn14;
    private javax.swing.JButton jBtn15;
    private javax.swing.JButton jBtn16;
    private javax.swing.JButton jBtn17;
    private javax.swing.JButton jBtn18;
    private javax.swing.JButton jBtn2;
    private javax.swing.JButton jBtn3;
    private javax.swing.JButton jBtn4;
    private javax.swing.JButton jBtn5;
    private javax.swing.JButton jBtn6;
    private javax.swing.JButton jBtn7;
    private javax.swing.JButton jBtn8;
    private javax.swing.JButton jBtn9;
    private javax.swing.JTextField jtxtDisplay;
    // End of variables declaration                   
}
