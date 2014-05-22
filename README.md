pruebas
=======
package Programacion;

import java.awt.FlowLayout;
import java.awt.GridLayout;

import javax.swing.JButton;
import javax.swing.JComboBox;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;
import javax.swing.JRadioButton;
import javax.swing.JTabbedPane;
import javax.swing.JTextArea;
import javax.swing.JTextField;

public class Automovil extends JFrame{


	private JPanel panelAux,panelAux1,paneldatosVehiculo,paneldatosRegistro;
	private JLabel lbldatosvehiculos,lbldatosper,lblplacas,lblserial_motor,lblserial_carr,lblaÃ±o,lblmarca,lblmodelo,
					lblnum_puertas,lblmotorcc,lblcarburado,lblobservacion;
	private JTextField txtplacas,txtserial_motor,txtserial_carr,txtaÃ±o,txtnum_puertas,txtmotorcc;
	private JRadioButton RbtnSi,RbtnNo;
	private JButton btnguardar,btnimprimir,btneliminar,btncerrar;
	private JComboBox combomarca, combomodelo;
	private JTextArea txtAobservacion;
	
		public Automovil(){
			
			//inicializar
		
			lbldatosvehiculos=new JLabel("Datos Vehiculo:");
			lblplacas=new JLabel ("Placas:");
			lblserial_motor=new JLabel ("Serial Motor:");
			lblserial_carr=new JLabel ("Serial Carroceria:");
			lblaÃ±o=new JLabel ("AÃ±o:");
			lblmarca=new JLabel ("Marca:");
			lblmodelo=new JLabel ("Modelo:");
			lblnum_puertas=new JLabel ("NÂº Puertas:");
			lblmotorcc=new JLabel ("MotorCC:");
			lblcarburado=new JLabel ("Carburado:");
			lblobservacion=new JLabel ("Observacion:");
			txtplacas=new JTextField(8);
			txtserial_motor=new JTextField(20);
			txtserial_carr=new JTextField(20);
			txtaÃ±o=new JTextField(4);
			txtnum_puertas=new JTextField(4);
			txtmotorcc=new JTextField(2);
			RbtnSi=new JRadioButton("Si");
			RbtnNo=new JRadioButton("No");
			btnguardar=new JButton("Guardar");
			btnimprimir=new JButton("Imprimir");
			btneliminar=new JButton("Eliminar");
			btncerrar=new JButton("Cerrar");
			txtAobservacion=new JTextArea(3,10);
			
			//combo box
			
			String[] marcas={"Fiat","Ford","Chevrolet","Chery","JAMS"};
			combomarca=new JComboBox(marcas);
			
			String[] modelo={"Sedan","CoupÃ©","Deportivo","Pickup"};
			combomodelo=new JComboBox(modelo);
			
			// Panel Datos Vehiculo
			
			paneldatosVehiculo=new JPanel(new GridLayout(6,1));
			paneldatosVehiculo.add(lbldatosvehiculos);
			
			panelAux=new JPanel(new FlowLayout());
			panelAux.add(lblplacas);
			panelAux.add(txtplacas);
			panelAux.add(lblserial_motor);
			panelAux.add(txtserial_motor);
			panelAux.add(lblserial_carr);
			panelAux.add(txtserial_carr);
			
			paneldatosVehiculo.add(panelAux);
			
			
			panelAux=new JPanel(new FlowLayout());
			panelAux.add(lblaÃ±o);
			panelAux.add(txtaÃ±o);
			panelAux.add(lblmarca);
			panelAux.add(combomarca);
			panelAux.add(lblmodelo);
			panelAux.add(combomodelo);
			panelAux.add(lblnum_puertas);
			panelAux.add(txtnum_puertas);

			paneldatosVehiculo.add(panelAux);
			
			panelAux=new JPanel(new FlowLayout());
			panelAux.add(lblmotorcc);
			panelAux.add(txtmotorcc);
			panelAux.add(lblcarburado);
			panelAux.add(RbtnSi);
			panelAux.add(RbtnNo);
			
			paneldatosVehiculo.add(panelAux);
			
			panelAux=new JPanel(new FlowLayout());
			panelAux.add(lblobservacion);
			panelAux.add(txtAobservacion);
			
			paneldatosVehiculo.add(panelAux);
			
			panelAux=new JPanel(new FlowLayout());
			panelAux.add(btnguardar);
			panelAux.add(btnimprimir);
			panelAux.add(btneliminar);
			panelAux.add(btncerrar);
			
			paneldatosVehiculo.add(panelAux);//Fin de Panel datosVehiculos
			
			//paneldatosRegistro=new JPanel(new GridLayout(4,1));//inicializando
			
			
			this.add(paneldatosVehiculo);
			this.pack();
			this.setLocationRelativeTo(null);
			this.setVisible(true);
		}
	
	
	
	public static void main(String[] args) {
		new Automovil();
	}

}
