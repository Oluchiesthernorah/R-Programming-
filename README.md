# R-Programming-
Data structure explains or teaches how data is represented.
 Essentially, we have 4 data structure:
 1. Vector
 2. Matrices
 3. Lists
 4. Dataframe

 '''
#VECTOR: this is defined as one dimensional array that holds data of the type
 #eg numeric, Character and logic.
 #Vector Function is written as c()
 #for example
 
 #Numeric Vector
 Vesther<- c(7, 4, 6, 1, 0)
 # LET US WORK WITH NUMERIC VECTOR
 Vesther*7 # multiplies the entire vector by 7
#To call out an element from vector use  []
 Vesther[2] #2 written in a square bracket is referring to positioning not a figure
 Vesther[2]*2 
 Vesther[c(1, 3)] #calling out multiple elements in a vector
 Vesther[-4] #To remove element in position 4
 Vesther[3]<-78 #To assign element in position 3 to be 78
 Vesther<- c(Vesther, 67) #To add 67 to the vector Vesther
 
 #Character vector
 Cesther<- c("oranges", "Banana", "Tangerine", 'Berry')

 #Logical Vector
 Lesther<-c (TRUE, FALSE, FALSE, TRUE)


#MATRICES
#This is defined as two dimensional array that holds data of the same type.
(#Matrices function is written as Matrix())
  
  #Let us create our first matrix
  EstherM<- matrix(c(1, 2, 3, 4, 5, 6), nrow=2, ncol=3)

  #let us call out elements in the first row and third column
  EstherM [1,3]

  #To access a row
  EstherM[2, ]

  #To access a column
  EstherM[ ,2]

  #To modify/change element in second row and third column
  EstherM[2,3]<-10

  #To add another row in the matrix
  New_EstherM <- c(12, 23, 34)
  EsrherM<-rbind(EstherM, New_EstherM)
  
  # to transpose Matrix
  t(EstherM)
  
#List  
#List: This data structure holds different form of data type, usually associated to a particular character
  #List Function is written as list()
  
  EstherL<-list(name = "Esty", Age = 25, Scores = c(92, 96, 88))
  EstherL$name #$ is used to call out a list
  EstherL$Age
  EstherL$Scores
  EstherL$Age<-30
  #to add another feature to the EstherL(list of Esther) like country
  EstherL$Country<-"Nigeria"
  
#Dataframe
 #Dataframe: This data structure holds different form of data type, usually associated to a multiple character
  #Dataframe Function is written as data.frame()
Estherdf<-data.frame(
    Name= c("Yewande", "David", "Yemi", "Kelvin"),
    Age= c(25, 26, 27, 28),
    Score= c(96, 97, 98, 99)
)

Estherdf$Name
Estherdf$Age
Estherdf$score
Estherdf[1, ] #To call out what you have in the first row
Estherdf[3,2] #To call out what you have in the third row and second column
Estherdf$Country<- c("Kenya", "UK", "Nigeria", "Ghana") #Adding a new column
