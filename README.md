# Bulldozer-Price-prediction-Model
This is a ML implementation for predicting bulldozer's price.


"""
Below is the description of all the variables from the dataset 
"""
Variable	Description
SalesID	  unique identifier of a particular sale of a machine at auction
MachineID	  identifier for a particular machine;  machines may have multiple sales
ModelID	  identifier for a unique machine model (i.e. fiModelDesc)
datasource	  source of the sale record;  some sources are more diligent about reporting attributes of the machine than others.  Note that a particular datasource may report on multiple auctioneerIDs.
auctioneerID	  identifier of a particular auctioneer, i.e. company that sold the machine at auction.  Not the same as datasource.
YearMade	  year of manufacturer of the Machine
MachineHoursCurrentMeter	  current usage of the machine in hours at time of sale (saledate);  null or 0 means no hours have been reported for that sale
UsageBand	  value (low, medium, high) calculated comparing this particular Machine-Sale hours to average usage for the fiBaseModel;  e.g. 'Low' means this machine has less hours given it's lifespan relative to average of fiBaseModel.
Saledate	  time of sale
Saleprice	  cost of sale in USD
fiModelDesc	  Description of a unique machine model (see ModelID); concatenation of fiBaseModel & fiSecondaryDesc & fiModelSeries & fiModelDescriptor
fiBaseModel	  disaggregation of fiModelDesc
fiSecondaryDesc	  disaggregation of fiModelDesc
fiModelSeries	  disaggregation of fiModelDesc
fiModelDescriptor	  disaggregation of fiModelDesc
ProductSize	  Don't know what this is 
ProductClassDesc	  description of 2nd level hierarchical grouping (below ProductGroup) of fiModelDesc
State	  US State in which sale occurred
ProductGroup	  identifier for top-level hierarchical grouping of fiModelDesc
ProductGroupDesc	  description of top-level hierarchical grouping of fiModelDesc
Drive_System	machine configuration;  typcially describes whether 2 or 4 wheel drive
Enclosure	machine configuration - does machine have an enclosed cab or not
Forks	machine configuration - attachment used for lifting
Pad_Type	machine configuration - type of treads a crawler machine uses
Ride_Control	machine configuration - optional feature on loaders to make the ride smoother
Stick	machine configuration - type of control 
Transmission	machine configuration - describes type of transmission;  typically automatic or manual
Turbocharged	machine configuration - engine naturally aspirated or turbocharged
Blade_Extension	machine configuration - extension of standard blade
Blade_Width	machine configuration - width of blade
Enclosure_Type	machine configuration - does machine have an enclosed cab or not
Engine_Horsepower	machine configuration - engine horsepower rating
Hydraulics	machine configuration - type of hydraulics
Pushblock	machine configuration - option
Ripper	machine configuration - implement attached to machine to till soil
Scarifier	machine configuration - implement attached to machine to condition soil
Tip_control	machine configuration - type of blade control
Tire_Size	machine configuration - size of primary tires
Coupler	machine configuration - type of implement interface
Coupler_System	machine configuration - type of implement interface
Grouser_Tracks	machine configuration - describes ground contact interface
Hydraulics_Flow	machine configuration - normal or high flow hydraulic system
Track_Type	machine configuration - type of treads a crawler machine uses
Undercarriage_Pad_Width	machine configuration - width of crawler treads
Stick_Length	machine configuration - length of machine digging implement
Thumb	machine configuration - attachment used for grabbing
Pattern_Changer	machine configuration - can adjust the operator control configuration to suit the user
Grouser_Type	machine configuration - type of treads a crawler machine uses
Backhoe_Mounting	machine configuration - optional interface used to add a backhoe attachment
Blade_Type	machine configuration - describes type of blade
Travel_Controls	machine configuration - describes operator control configuration
Differential_Type	machine configuration - differential type, typically locking or standard
Steering_Controls	machine configuration - describes operator control configuration
