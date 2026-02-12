<img width="487" height="240" alt="image" src="https://github.com/user-attachments/assets/e6a1e312-8127-4e3d-9959-4823d6b8fa23" />
<img width="376" height="237" alt="image" src="https://github.com/user-attachments/assets/a1a05f85-81ab-4f1c-9a81-613a2692aca0" />

import javax.swing.*; import java.awt.event.ActionEvent; import java.awt.event.ActionListener;


public class tombolinteraktif extends javax.swing.JFrame {

    
    public tombolinteraktif() {
        // Set judul frame
        setTitle ("tombolinteraktif");
        initComponents();
        
        // Set ukuran frame
        setSize(500,250);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null); 
        
        //buat Jlabel
        JLabel label = new JLabel("Halo, Nama saya!");
    label.setBounds(50, 50, 250, 30);

    // buat JButton
     JButton button = new JButton("tekan saya");
    button.setBounds(50, 100, 200, 30);
    
    
      // Tambahkan ActionListener pada tombol
    button.addActionListener(new ActionListener() {
        @Override
        public void actionPerformed(ActionEvent e) {
            label.setText("Mentari Putri Sanggor");
        }
    });
     
     // Tambahkan komponen ke frame 
    add(label);
    add(button);
    
     // Set layout menjadi null agar bisa atur posisi manual
    setLayout(null);
    }

    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">                          
    private void initComponents() {

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

        javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
        getContentPane().setLayout(layout);
        layout.setHorizontalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGap(0, 373, Short.MAX_VALUE)
        );
        layout.setVerticalGroup(
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
            .addGap(0, 300, Short.MAX_VALUE)
        );

        pack();
    }// </editor-fold>                        

    
    public static void main(String args[]) {
      tombolinteraktif frame = new tombolinteraktif();
      frame.setVisible(true);
        java.awt.EventQueue.invokeLater(new Runnable() {
            public void run() {
                new tombolinteraktif().setVisible(true);
            }
        });
    }

    // Variables declaration - do not modify                     
    // End of variables declaration                   
}

