package VistaCalculadora;


import java.awt.BorderLayout;
import java.awt.Color;
import java.awt.FlowLayout;
import java.awt.GridBagLayout;
import java.awt.GridLayout;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JMenu;
import javax.swing.JMenuBar;
import javax.swing.JMenuItem;
import javax.swing.JPanel;
import javax.swing.JTextArea;
import javax.swing.border.LineBorder;
import javax.swing.border.TitledBorder;

public class Calculadora extends JFrame {

	private JPanel panelVisor,panelPantalla,
				panelAux,panelBotones,panelMarca;
	private JTextArea txtVisor;
	private JButton btnBoton7,btnBoton8,btnBoton9,
			btnBotonDel,btnBotonAc,
			btnBoton4,btnBoton5,btnBoton6,btnBotonX,btnBotonDiv,
			btnBoton1,btnBoton2,btnBoton3,btnBotonS,btnBotonR,
			btnBoton0,btnBotonP,btnBotonE,btnBotonAns,btnBotonI;
	private JMenuBar barraMenu;
	private JMenu mEdit,mVarios;
	private JMenuItem mE_Copiar,mE_Cortar,mE_Pegar,
					  mV_Acerca,mV_Cerrar;
	private JLabel lblMarca;
	public Calculadora(){
		//inicializar objetos
		txtVisor=new JTextArea(3,20);
		lblMarca=new JLabel("UNERG");
		//botones
		btnBoton7=new JButton("7");
		btnBoton8=new JButton("8");
		btnBoton9=new JButton("9");
		btnBotonDel=new JButton("Del");
		btnBotonAc=new JButton("AC");
		
		btnBoton4=new JButton("4");
		btnBoton5=new JButton("5");
		btnBoton6=new JButton("6");
		btnBotonX=new JButton("X");
		btnBotonDiv=new JButton("/");
		
		btnBoton1=new JButton("1");
		btnBoton2=new JButton("2");
		btnBoton3=new JButton("3");
		btnBotonS=new JButton("+");
		btnBotonR=new JButton("-");
		
		btnBoton0=new JButton("0");
		btnBotonP=new JButton(".");
		btnBotonE=new JButton("EXP");
		btnBotonAns=new JButton("Ans");
		btnBotonI=new JButton("=");
		
		
		//definir panel visor y ensamblar
		panelVisor=new JPanel();
		panelPantalla=new JPanel();
		panelVisor.setBorder(new TitledBorder("AIS"));

		
		panelPantalla.setBorder
				(new LineBorder(Color.BLUE,1,true));

		panelPantalla.add(txtVisor);
		
		panelVisor.add(panelPantalla);
		
		//ensamblar panelBotones
		
		panelBotones=new JPanel(new GridLayout(4,5));
		
		//linea 1
		
		panelBotones.add(btnBoton7);
		panelBotones.add(btnBoton8);
		panelBotones.add(btnBoton9);
		panelBotones.add(btnBotonDel);
		panelBotones.add(btnBotonAc);
		

		
		//linea 2
	
		panelBotones.add(btnBoton4);
		panelBotones.add(btnBoton5);
		panelBotones.add(btnBoton6);
		panelBotones.add(btnBotonX);
		panelBotones.add(btnBotonDiv);
		
		//linea 3
		
		panelBotones.add(btnBoton1);
		panelBotones.add(btnBoton2);
		panelBotones.add(btnBoton3);
		panelBotones.add(btnBotonS);
		panelBotones.add(btnBotonR);
			
	//linea 4
		
		panelBotones.add(btnBoton0);
		panelBotones.add(btnBotonP);
		panelBotones.add(btnBotonE);
		panelBotones.add(btnBotonAns);
		panelBotones.add(btnBotonI);
		
		panelAux=new JPanel();
		panelAux.setBorder
		(new LineBorder(Color.BLUE,2,true));
		panelAux.add(panelBotones);
		
		//menu editar
		mEdit=new JMenu("Editar");
		mEdit.setMnemonic('E');
		
		mE_Copiar=new JMenuItem("Copiar");
		mE_Cortar=new JMenuItem("Cortar");
		mE_Pegar=new JMenuItem("Pegar");
		mEdit.add(mE_Copiar);
		mEdit.add(mE_Cortar);
		mEdit.add(mE_Pegar);
		
		//menu varios
		mVarios=new JMenu("Varios");
		mVarios.setMnemonic('V');
		
		mV_Acerca=new JMenuItem("Acerca de");
		mV_Cerrar=new JMenuItem("Cerrar");
		
		mVarios.add(mV_Acerca);
		mVarios.add(mV_Cerrar);
		
		//ensamblar barra de menu
		barraMenu=new JMenuBar();
		barraMenu.add(mEdit);
		barraMenu.add(mVarios);
		
		this.setJMenuBar(barraMenu);
		
		//panel Marca
		
		panelMarca=new JPanel(new FlowLayout(FlowLayout.RIGHT));
		panelMarca.add(lblMarca);
		
		
		//calculadora
		this.add(panelVisor,BorderLayout.NORTH);
		this.add(panelAux,BorderLayout.CENTER);
		this.add(panelMarca,BorderLayout.SOUTH);
		//this.setSize(300, 270);
		this.pack();
		this.setLocationRelativeTo(null);
		this.setVisible(true);
		
		
		
		
	}
	public static void main(String[] args) {
		new Calculadora();

	}

}
