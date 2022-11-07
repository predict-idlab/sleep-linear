## Impact of various input signal combinations on performance 


Summary of the results from the `inputs_`* notebooks.

<table>
<thead>
  <tr>
    <th>Dataset</th>
    <th>System</th>
    <th>Signals</th>
    <th>MF1</th>
    <th>ACC</th>
    <th>kAPPA</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="8">Sleep-EDF-SC-20</td>
    <td rowspan="4">Logistic regr.</td>
    <td>EEG</td>
    <td>0.780</td>
    <td>0.839</td>
    <td>0.781</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0.787</td>
    <td>0.842</td>
    <td>0.884</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0.803</td>
    <td>0.853</td>
    <td>0.800</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0.809</td>
    <td>0.857</td>
    <td>0.806</td>
  </tr>
  <tr>
    <td rowspan="4">Catboost</td>
    <td>EEG</td>
    <td>0.772</td>
    <td>0.842</td>
    <td>0.782</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0.774</td>
    <td>0.842</td>
    <td>0.782</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0.797</td>
    <td>0.860</td>
    <td>0.807</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0.802</td>
    <td>0.864</td>
    <td>0.812</td>
  </tr>
  <tr>
    <td rowspan="8">Sleep-EDF-SC-78</td>
    <td rowspan="4">Logistic regr.</td>
    <td>EEG</td>
    <td>0.738</td>
    <td>0.797</td>
    <td>0.723</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0.746</td>
    <td>0.800</td>
    <td>0.728</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0.768</td>
    <td>0.820</td>
    <td>0.753</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0,771</td>
    <td>0,821</td>
    <td>0,756</td>
  </tr>
  <tr>
    <td rowspan="4">Catboost</td>
    <td>EEG</td>
    <td>0.745</td>
    <td>0.810</td>
    <td>0.736</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0,750</td>
    <td>0,813</td>
    <td>0,741</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0.772</td>
    <td>0,830</td>
    <td>0,763</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0,775</td>
    <td>0,831</td>
    <td>0,766</td>
  </tr>
  <tr>
    <td rowspan="8">Sleep-EDF-ST</td>
    <td rowspan="4">Logistic regr.</td>
    <td>EEG</td>
    <td>0,758</td>
    <td>0,802</td>
    <td>0,723</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0,776</td>
    <td>0,816</td>
    <td>0,741</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0,788</td>
    <td>0,825</td>
    <td>0,754</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0,792</td>
    <td>0,829</td>
    <td>0,759</td>
  </tr>
  <tr>
    <td rowspan="4">Catboost</td>
    <td>EEG</td>
    <td>0,771</td>
    <td>0,821</td>
    <td>0,744</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0,784</td>
    <td>0,829</td>
    <td>0,755</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0,789</td>
    <td>0,832</td>
    <td>0,758</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0,795</td>
    <td>0,836</td>
    <td>0,765</td>
  </tr>
  <tr>
    <td rowspan="8">MASS SS3</td>
    <td rowspan="4">Logistic regr.</td>
    <td>EEG</td>
    <td>0,793</td>
    <td>0,844</td>
    <td>0,774</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0,803</td>
    <td>0,850</td>
    <td>0,782</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0,794</td>
    <td>0,845</td>
    <td>0,775</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0,807</td>
    <td>0,853</td>
    <td>0,786</td>
  </tr>
  <tr>
    <td rowspan="4">Catboost</td>
    <td>EEG</td>
    <td>0,810</td>
    <td>0,863</td>
    <td>0,796</td>
  </tr>
  <tr>
    <td>EEG + EMG</td>
    <td>0,815</td>
    <td>0,864</td>
    <td>0,798</td>
  </tr>
  <tr>
    <td>EEG + EOG</td>
    <td>0,809</td>
    <td>0,863</td>
    <td>0,797</td>
  </tr>
  <tr>
    <td>EEG + EOG + EMG</td>
    <td>0,817</td>
    <td>0,867</td>
    <td>0,803</td>
  </tr>
</tbody>
</table>
