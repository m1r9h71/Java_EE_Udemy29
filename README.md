# Java_EE_Udemy29
One to One relationship between Flight and Airplane
In Flight:
    	  @OneToOne //shows relationship between the two tables
	  @JoinColumn(name= "airplane_fk")//joins using airplane foreign key
	  private Airplane airplaneDetail; //creates the variable to join the two

In Airplane:
          @OneToOne(mappedBy = "airplaneDetail") //joins the variable in Flight
	  private Flight flight; //creates the variable
    
    
