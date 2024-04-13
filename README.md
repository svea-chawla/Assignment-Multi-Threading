# Assignment-Multi-Threading
Objective:
The goal is to conduct matrix multiplication on 100 matrices sized 1000 X 1000 using various thread counts and visualize the time taken and CPU usage.

Methodology:
Matrix Multiplication: The multiply() function performs matrix multiplication on matrices A and B using np.dot(), storing the result in a designated index of the result array.

Thread Utilization: The run_threads() function is implemented to execute matrix multiplication using a variable number of threads (1-10). It initializes a list called threads to store thread objects. It iterates over the list of matrices, creating a new thread for each matrix multiplication operation using the threading.Thread() constructor. Each thread is started using the start() method. After creating all threads, it waits for all threads to complete using the join() method and returns the time taken for the multiplication operations.

Matrix Generation: A constant matrix A of size 1000x1000 is generated using numpy.random.rand(). A list of 100 random matrices of the same size is then created.

Execution: The run_threads() function is invoked for each number of threads ranging from 1 to 10, recording the time taken for each operation. The results are stored in the results_table list along with the corresponding number of threads.

Results: The results are presented in tabular format using tabulate(). The number of threads is plotted against the corresponding time taken using matplotlib.pyplot.plot().

We observe that the minimum time is taken when the the number of threads are 1.

![image](https://github.com/svea-chawla/Assignment-Multi-Threading/assets/111569685/ad8a1abb-f0b8-4ad3-b358-11e04f5d1abe)

![image](https://github.com/svea-chawla/Assignment-Multi-Threading/assets/111569685/1db4b554-ef2d-4ccc-a300-1c38aa05271c)
