Review Assignment Due Date
Assignment1
Imagine you're building a car fleet management system. Start by developing a class named Car. Inside this class, you should have two private data members. The first is modelName, which will be a String representing the name of the car model. The second is fuelEfficiency, a double that captures the car's fuel efficiency in terms of miles per gallon or km per liter. The class should have a constructor. This constructor should accept two arguments, initializing the modelName and fuelEfficiency accordingly.

The class should also provide a public method named getFuelEfficiency that returns the current value of the fuelEfficiency data member. To be able to change this data member, create another public method named setFuelEfficiency which allows one to modify the value of the fuelEfficiency. Once your Car class is ready, create another class named EfficiencyStats. This class should offer a public static method named computeStats. This method will be responsible for computing the mean, median, and mode of the fuel efficiencies of a list of cars. It should take an ArrayList as its only parameter and return these computed statistics in an instance of a custom class named StatsResult. This StatsResult class should provide three data members: mean, median, and mode. To illustrate the functionality of your classes, one should be able to interact with them as follows:

Car car1 = new Car("Tesla Model S", 90.9); 
Car car2 = new Car("Toyota Prius", 56.5); 
Car car3 = new Car("Honda Civic", 32.3); 
Car car4 = new Car("Ford Mustang", 25.5); 
ArrayList<Car> carList = new ArrayList<>(Arrays.asList(car1, car2, car3, car4)); 
StatsResult result = EfficiencyStats.computeStats(carList); 
System.out.println(result.mean);
System.out.println(result.median); 
System.out.println(result.mode);
