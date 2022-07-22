README.md

Run with the bash command 'python3 stocksRNN.py' as any other Python file.

Output will occasionally overflow and give results of NaN.  This happens somewhat randomly due to random initialization of weights.  This is most likely to happen if you choose an unecessarily high hidden layer size or a learning rate that is too high.  If this happens, please just be patient and try it a couple more times.

There is a warning concerning the line "close_prices = close_prices[:, np.newaxis]".  It does not currently interfere with the program's function and research into the message gave no useful results and an alternative could not be found.  It may need to be fixed at a later date.
 FutureWarning: Support for multi-dimensional indexing (e.g. `obj[:, None]`) is deprecated and will be removed in a future version.  Convert to a numpy array before indexing instead.
  close_prices = close_prices[:, np.newaxis]

One of this program's weaknesses is its inability to predict more than 1 day in the future.  More advanced techniques would have to be implemented to predict multiple timesteps of data without the actual value of the previous timestep.  This prediction of multiple timesteps is a potential subject of future work.