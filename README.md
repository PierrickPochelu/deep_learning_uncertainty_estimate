# deep_learning_uncertainty_estimate



## Standard CNN
 <table>
  <tr>
    <th>Method</th>
    <th>#Training</th>
    <th>#Predicting</th>
    <th>Accuracy</th>
    <th>Cross entropy</th>
    <th>ECE</th>
    <th>Brier</th>
  </tr>
    <tr>
    <td>Standard CNN</td>
    <td>1</td>
    <td>1</td>
    <td>0.5368</td>
    <td>0.2005</td>
    <td>0.3844</td>
    <td>0.5932</td>
  </tr>
  </table>
  
  ## Deep ensemble
URL: https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf
  <table>
    <tr>
    <th>Method</th>
    <th>#Training</th>
    <th>#Predicting</th>
    <th>Accuracy</th>
    <th>Cross entropy</th>
    <th>ECE</th>
    <th>Brier</th>
  </tr>
  <tr><td>Ensemble</td><td>1</td><td>1</td><td>0.5353</td><td>0.2021</td><td>0.3782</td><td>0.5967</td></tr>
<tr><td>Ensemble</td><td>2</td><td>2</td><td>0.5757</td><td>0.1876</td><td>0.4212</td><td>0.5535</td></tr>
<tr><td>Ensemble</td><td>3</td><td>3</td><td>0.5761</td><td>0.1881</td><td>0.424</td><td>0.5555</td></tr>
<tr><td>Ensemble</td><td>4</td><td>4</td><td>0.5776</td><td>0.1885</td><td>0.4262</td><td>0.5569</td></tr>
<tr><td>Ensemble</td><td>5</td><td>5</td><td>0.5786</td><td>0.1883</td><td>0.4279</td><td>0.5561</td></tr>
<tr><td>Ensemble</td><td>6</td><td>6</td><td>0.5789</td><td>0.1877</td><td>0.4281</td><td>0.5548</td></tr>
<tr><td>Ensemble</td><td>7</td><td>7</td><td>0.5828</td><td>0.1863</td><td>0.4316</td><td>0.55</td></tr>
<tr><td>Ensemble</td><td>8</td><td>8</td><td>0.5855</td><td>0.1864</td><td>0.4346</td><td>0.5502</td></tr>
<tr><td>Ensemble</td><td>9</td><td>9</td><td>0.586</td><td>0.186</td><td>0.4355</td><td>0.5492</td></tr>
<tr><td>Ensemble</td><td>10</td><td>10</td><td>0.5883</td><td>0.1856</td><td>0.4379</td><td>0.5477</td></tr>
<tr><td>Ensemble</td><td>11</td><td>11</td><td>0.5901</td><td>0.1854</td><td>0.4398</td><td>0.5471</td></tr>
<tr><td>Ensemble</td><td>12</td><td>12</td><td>0.595</td><td>0.1846</td><td>0.4447</td><td>0.5444</td></tr>
<tr><td>Ensemble</td><td>13</td><td>13</td><td>0.5963</td><td>0.185</td><td>0.4467</td><td>0.5453</td></tr>
<tr><td>Ensemble</td><td>14</td><td>14</td><td>0.5951</td><td>0.185</td><td>0.4456</td><td>0.5455</td></tr>
<tr><td>Ensemble</td><td>15</td><td>15</td><td>0.597</td><td>0.1843</td><td>0.4474</td><td>0.5432</td></tr>
<tr><td>Ensemble</td><td>16</td><td>16</td><td>0.5981</td><td>0.1842</td><td>0.4484</td><td>0.5431</td></tr>
  </table>
<table>

## MC-dropout
 RL: https://arxiv.org/pdf/1506.02142.pdf
MC-droupout. The dropout is varied (50%, 5%, 0.5%, 0.2%) and the number of averaged predictions (4, 8, 16, 32).
  <table>
    <tr>
    <th>Method</th>
    <th>#Training</th>
    <th>#Predicting</th>
    <th>Accuracy</th>
    <th>Cross entropy</th>
    <th>ECE</th>
    <th>Brier</th>
  </tr>
<tr><td>MC-drop rate=0.5</td><td>1</td><td>4</td><td>0.4713</td><td>0.2244</td><td>0.3341</td><td>0.6615</td></tr>
<tr><td>MC-drop rate=0.5</td><td>1</td><td>8</td><td>0.4746</td><td>0.2227</td><td>0.3381</td><td>0.6567</td></tr>
<tr><td>MC-drop rate=0.5</td><td>1</td><td>16</td><td>0.4777</td><td>0.2219</td><td>0.3416</td><td>0.6542</td></tr>
<tr><td>MC-drop rate=0.5</td><td>1</td><td>32</td><td>0.4765</td><td>0.2216</td><td>0.3406</td><td>0.6532</td></tr>
<tr><td>MC-drop rate=0.05</td><td>1</td><td>4</td><td>0.5496</td><td>0.195</td><td>0.3923</td><td>0.5783</td></tr>
<tr><td>MC-drop rate=0.05</td><td>1</td><td>8</td><td>0.548</td><td>0.1948</td><td>0.3909</td><td>0.5777</td></tr>
<tr><td>MC-drop rate=0.05</td><td>1</td><td>16</td><td>0.5503</td><td>0.1947</td><td>0.3932</td><td>0.5772</td></tr>
<tr><td>MC-drop rate=0.05</td><td>1</td><td>32</td><td>0.5504</td><td>0.1945</td><td>0.3934</td><td>0.5769</td></tr>
<tr><td>MC-drop rate=0.005</td><td>1</td><td>4</td><td>0.5337</td><td>0.2036</td><td>0.3801</td><td>0.6006</td></tr>
<tr><td>MC-drop rate=0.005</td><td>1</td><td>8</td><td>0.5337</td><td>0.2035</td><td>0.3801</td><td>0.6002</td></tr>
<tr><td>MC-drop rate=0.005</td><td>1</td><td>16</td><td>0.5344</td><td>0.2035</td><td>0.3808</td><td>0.6001</td></tr>
<tr><td>MC-drop rate=0.005</td><td>1</td><td>32</td><td>0.5339</td><td>0.2035</td><td>0.3803</td><td>0.6001</td></tr>
<tr><td>MC-drop rate=0.002</td><td>1</td><td>4</td><td>0.5495</td><td>0.1951</td><td>0.3933</td><td>0.5785</td></tr>
<tr><td>MC-drop rate=0.002</td><td>1</td><td>8</td><td>0.5495</td><td>0.1951</td><td>0.3933</td><td>0.5785</td></tr>
<tr><td>MC-drop rate=0.002</td><td>1</td><td>16</td><td>0.5489</td><td>0.195</td><td>0.3927</td><td>0.5784</td></tr>
<tr><td>MC-drop rate=0.002</td><td>1</td><td>32</td><td>0.5485</td><td>0.195</td><td>0.3923</td><td>0.5783</td></tr>
 </table>
A small dropout match a standard neural network accuracy/uncertainty. No significant difference between 16 predictions and 32. 
  
 ## Variational inference

Deep variational inference with Tensorflow_Probability (TFP) 
<table>
    <tr>
    <th>Method</th>
    <th>#Training</th>
    <th>#Predicting</th>
    <th>Accuracy</th>
    <th>Cross entropy</th>
    <th>ECE</th>
    <th>Brier</th>
  </tr>

<tr><td>1layer</td><td>1</td><td>4</td><td>0.554</td><td>0.1949</td><td>0.3989</td><td>0.5749</td></tr>
<tr><td>1layer</td><td>1</td><td>16</td><td>0.5587</td><td>0.1942</td><td>0.404</td><td>0.5729</td></tr>
<tr><td>1layer TFP</td><td>1</td><td>64</td><td>0.5416</td><td>0.2017</td><td>nan</td><td>0.5971</td></tr>
<tr><td>2layers TFP</td><td>1</td><td>4</td><td>0.5537</td><td>0.1956</td><td>nan</td><td>0.577</td></tr>
<tr><td>2layers TFP</td><td>1</td><td>16</td><td>0.5556</td><td>0.1951</td><td>nan</td><td>0.5756</td></tr>
<tr><td>2layers TFP</td><td>1</td><td>64</td><td>0.5579</td><td>0.195</td><td>nan</td><td>0.575</td></tr>
</table> 

 
## Temperature scaling (TS)
 
 URL: :https://arxiv.org/pdf/1706.04599.pdf
 The validation/training split is varyied (r= 10%, 1%, 0.1%)
 
<table>
<tr>TS r=0.1<td>0.1</td><td>1</td><td>1</td><td>0.548</td><td>0.2585</td><td>0.4319</td><td>0.7265</td></tr>
<tr>TS r=0.01<td>0.01</td><td>1</td><td>1</td><td>0.5193</td><td>0.2612</td><td>0.4016</td><td>0.732</td></tr>
<tr>TS r=0.001<td>0.001</td><td>1</td><td>1</td><td>0.5665</td><td>0.2545</td><td>0.4494</td><td>0.7144</td></tr>
</table>
 
Compared to the standard CNN, ECE score is better but not the Brier. The ensemble of 16 have also a lower ECE than TS with r=0.001.
 
 ## Conclusion
Ensemble of Deep Neural Network seems the best method to build accuracy/uncertainty prediction at a given inference cost. However, they require to multiply the training time.
