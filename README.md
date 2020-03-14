# javaForm
This is a beginner level java form.






package com.company;
import javax.swing.*;
import javax.swing.border.Border;
import java.awt.*;

public class Main {
    private JFrame frame;
    private JLabel lbl1,lbl2,lbl3,lbl4,lbl5,lbl6,lbl7,lbl8,lbl9,lbl10,lbl11,lbl12,lbl13,lbl14,lbl15,lbl16,lbl17,lbl18;
    private JButton btn1, btn2, btn3, btn4, btn5,btn6 ;
    private JComboBox cb1, cb2, cb3,cb4;
    private JPanel p1, p2;
    private JTextArea txt1, txt2, txt3 , txt4, txt5,txt6,txt7,txt8,txt9,txt10,txt11;

    public static void main(String[] args) {
	    new Main();
    }
    public Main(){
        frame= new JFrame("This is a Frame");
        frame.setLayout(null);
        frame.setSize(1000,600);
        frame.setLayout(null);
        frame.setResizable(false);
        frame.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);

        //setting up panel for the Header
        p1= new JPanel();
        p1.setLayout(null);
        p1.setBounds(0,0,1000,100);
        //Header Label
        lbl1= new JLabel("Student's Registration Form");
        Font f= new Font("null",Font.PLAIN,20);
        lbl1.setBounds(350,25,300,46);
        lbl1.setFont(f);
        p1.add(lbl1);
        //panel 2 for the components
        //For each and every components must be added to this panel..
        p2=new JPanel();
        p2.setLayout(null);
        p2.setBounds(0,100,1000,500);
        //Adding components in panel 2:
        lbl2= new JLabel("Student ID:");
        lbl2.setBounds(10,0,100,100);
        txt1= new JTextArea();
        txt1.setBounds(90,30,150,30);
        p2.add(lbl2);
        p2.add(txt1);
        //Making every components First:
        //labels
        lbl3= new JLabel("First Name:");
        lbl4= new JLabel("Last Name:");
        lbl5= new JLabel("Middle Name:");
        lbl6=new JLabel("Address:");
        //For the Combo Box School Year
        lbl7= new JLabel("School Year : ");
        lbl7.setBounds(660,0, 100,100);
        String[] Year={"2013-2014", "2012-2013", "2012-2011", "2011-2010"};
        cb1=new JComboBox(Year);
        cb1.setBounds(750,33,90,30);
        
        //For other parts of the GUI
        lbl8=  new JLabel("Place of Birth:");
        txt6=new JTextArea();

        //creating the combo box for bithdate:
        lbl9=new JLabel("Date of Birth:");
        String[] Years={"2009","2008","2007","2006","2005","2004","2003","2002","2001","2000",
                "1999","1998","1997","1996","1995","1994","1993","1992","1991","1990"};
        cb2=new JComboBox(Years);

        txt2=new JTextArea();
        txt3=new JTextArea();
        txt4=new JTextArea();
        txt5= new JTextArea();
        //setting the bounds of the labels and text area:

        lbl10=new JLabel("Age : ");
        txt7=new JTextArea();
        lbl11= new JLabel("Gender : " );
        JRadioButton r1=new JRadioButton(" Male");
        JRadioButton r2=new JRadioButton(" Female");
        ButtonGroup bg=new ButtonGroup();
        bg.add(r1);
        bg.add(r2);
        //
        lbl12=new JLabel("Status : ");
        String Status[]= {"Single","Married"};
        cb3=new JComboBox(Status);
        //
        lbl13=new JLabel("Year : ");
        String Sems[]= {"1st","2nd","3rd","4th"};
        cb4=new JComboBox(Sems);
        //
        lbl14=new JLabel("Guardian: ");
        txt8= new JTextArea();
        lbl15= new JLabel("Relation: ");
        txt9=new JTextArea();
        lbl16= new JLabel("Address: ");
        txt10= new JTextArea();
        lbl17= new JLabel("Contact#: ");
        txt11= new JTextArea();
        //The bottom part of the form
        btn1= new JButton("Save");
        btn2= new JButton("|<");
        btn3= new JButton("<<");
        btn4=new JButton(">>");
        btn5=new JButton(">|");
        btn6=new JButton("New");
        lbl18=new JLabel("0  OF  0" );
        //setting up bounds for the components:
        Border black=BorderFactory.createLineBorder(Color.BLACK);
        lbl3.setBounds(15,60,100,100);
        txt2.setBounds(90, 90, 150,30);
        lbl4.setBounds(350, 60, 100,100);
        txt3.setBounds(420, 95, 150,30);
        lbl5.setBounds(650, 60, 100,100);
        txt4.setBounds(750, 95, 150, 30);
        lbl6.setBounds(20, 120, 100,100);
        txt5.setBounds(90, 147, 150,50 );
        //lbl7 is set up already at the top :
        //lbl8 onwards:
        lbl8.setBounds(660, 120, 100,100);
        txt6.setBounds(750,145, 150,51);
        lbl9.setBounds(320, 120,100,100);
        cb2.setBounds(420,156,150,30);
        lbl10.setBounds(37,150,100,130);
        lbl11.setBounds(337,170,100,100);
        txt7.setBounds(89,205,70,30);
        r1.setBounds(400,180, 80,80);
        r2.setBounds(500,180,80,80);
        lbl12.setBounds(680,170,100,100);
        cb3.setBounds(750,202,100,30);
        lbl13.setBounds(37,222, 100,100);
        cb4.setBounds(90,255,70,30);
        lbl14.setBounds(320,223,100,100);
        txt8.setBounds(389,257,220,30);
        lbl15.setBounds(680,220,100,100);
        txt9.setBounds(740,255,150,30);
        lbl16.setBounds(30,285,100,100);
        txt10.setBounds(90,310,300,60);
        lbl17.setBounds(540,284,100,100);
        txt11.setBounds(650,320,250,30);
        btn1.setBounds(830,400,150,35);
        btn2.setBounds(10,400,80,27);
        btn3.setBounds(100,400,80,27);
        btn4.setBounds(210,400,80,27);
        btn5.setBounds(300,400,80,27);
        lbl18.setBounds(410,364,100,100);
        btn6.setBounds(720,400,80,35);

        //setting up black border for the text area
        txt1.setBorder(black);
        txt2.setBorder(black);
        txt3.setBorder(black);
        txt4.setBorder(black);
        txt5.setBorder(black);
        txt6.setBorder(black);
        txt7.setBorder(black);
        txt8.setBorder(black);
        txt9.setBorder(black);
        txt10.setBorder(black);
        txt11.setBorder(black);

        //adding the labels in panel:
        p2.add(lbl3);
        p2.add(txt2);
        p2.add(lbl4);
        p2.add(txt3);
        p2.add(lbl5);
        p2.add(txt4);
        p2.add(lbl6);
        p2.add(txt5);
        p2.add(cb1);
        p2.add(lbl7);
        p2.add(lbl8);
        p2.add(txt6);
        p2.add(lbl9);
        p2.add(cb2);
        p2.add(btn1);
        p2.add(lbl10);
        p2.add(lbl11);
        p2.add(txt7);
        p2.add(r1);
        p2.add(r2);
        p2.add(lbl12);
        p2.add(cb3);
        p2.add(lbl13);
        p2.add(cb4);
        p2.add(lbl14);
        p2.add(txt8);
        p2.add(lbl15);
        p2.add(txt9);
        p2.add(lbl16);
        p2.add(txt10);
        p2.add(lbl17);
        p2.add(txt11);
        p2.add(lbl18);
        p2.add(btn2);
        p2.add(btn3);
        p2.add(btn4);
        p2.add(btn5);
        p2.add(btn6);
        frame.add(p1);
        frame.add(p2);
        frame.setVisible(true);





    }






}

