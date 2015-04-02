import java.awt.Container;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JOptionPane;
import javax.swing.JPanel;


public class FrontEnd extends JFrame implements ActionListener
{
	private BackEnd backend;
	private Encoder encoder;
	private JButton addmessage;
	private JButton getmessage;
	
	public FrontEnd()
	{
		
		
		Container pane= this.getContentPane();
		backend= new BackEnd();
		encoder= new Encoder();
		addmessage = new JButton("add message");
		addmessage.setBounds(24, 94, 136, 37);
		getmessage = new JButton("get message");
		getmessage.setBounds(24, 11, 136, 37);
		
		
		
		addmessage.addActionListener(this);
		getmessage.addActionListener(this);
		
		addmessage.setActionCommand("addmessage");
		getmessage.setActionCommand("getmessage");
		
		this.setSize(200,200);
		getContentPane().setLayout(null);
		pane.add(addmessage);
		pane.add(getmessage);
		this.setVisible(true);
		
		
	}

	@Override
	public void actionPerformed(ActionEvent arg0) 
	{
		if(arg0.getActionCommand()=="addmessage")
		{
			Object[] bob= new Object[]{"Input Name", "Select Name"};
			int n= JOptionPane.showOptionDialog(this,"Select type of add",
				    	    "",
				    	    JOptionPane.YES_NO_OPTION,
				    	    JOptionPane.QUESTION_MESSAGE,
				    	    null,
				    	    bob,
				    	    bob[1]);
			if(n!=-1)
			{
				if(n==0)
				{
					String s= JOptionPane.showInputDialog("Type the Name");
				}
				else
				{
					String s = (String)JOptionPane.showInputDialog(
	                    frame,
	                    "Complete the sentence:\n"
	                    + "\"Green eggs and...\"",
	                    "Customized Dialog",
	                    JOptionPane.PLAIN_MESSAGE,
	                    icon,
	                    possibilities,
	                    "ham");
				}
			}
		}
		if(arg0.getActionCommand()=="getmessage")
		{
			
		}
		
		
	}
}
