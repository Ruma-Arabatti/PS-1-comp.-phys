import numpy as np

def f(x):
  return np.sin(x)

def Rectangle_Rule(f, x_min, x_max, N):
  x = np.linspace(x_min, x_max, N)
  dx = x[1] - x[0]
  Integral = 0
  for i in range(N-1):
    Integral += f(x[i])*dx   #area of rectangle
  return Integral

def Trapezoid_Rule(f, x_min, x_max, N):
  x = np.linspace(x_min, x_max, N)
  dx = x[1] - x[0]
  Integral = 0
  for i in range(N-1):
    Integral += 0.5*(f(x[i]) + f(x[i+1]))*dx  #area of trapezoid
  return Integral

def main():
  recthundred = Rectangle_Rule(f, 0, np.pi/2, 100)
  print("Value from the Rectangle Rule for 100 data points: " + str(recthundred))
  print("Error: " + str(1-recthundred))

  recttwohundred = Rectangle_Rule(f, 0, np.pi/2, 200)
  print("Value from the Rectangle Rule for 200 data points: " + str(recttwohundred))
  print("Error: " + str(1-recttwohundred))

  traphundred = Trapezoid_Rule(f, 0, np.pi/2, 100)
  print("Value from the Trapezoid Rule for 100 data points: " + str(traphundred))
  print("Error: " + str(1-traphundred))
  
  traptwohundred = Trapezoid_Rule(f, 0, np.pi/2, 200)
  print("Value from the Trapezoid Rule for 200 data points: " + str(traptwohundred))
  print("Error: " + str(1-traptwohundred))
  
if __name__ == "__main__":
    main()
