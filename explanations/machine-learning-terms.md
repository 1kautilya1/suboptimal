# Machine Learning Terms

Researchers often invent complicated names for simple things. This page will help you uncover the real meaning of those perplexing terms.

<table>
<thead>
<tr>
<th>Term</th>
<th>Human Language Translation</th>
</tr>
</thead>
<tbody>
<tr>
<td valign="top">Rectified Linear Unit (ReLU)</td>
<td>
    <p>A simple function of <tt>x</tt> returning 0 if <tt>x < 0</tt> or <tt>x</tt> otherwise</p>
    <p><img width="400px" src="images/relu.png"></p>
</td>
</tr>
<tr>
<td valign="top">Embedding</td>
<td>
    <p>A representation of an object as a list of numbers.</p>
    <p>Embeddings are commonly used to create representations of objects or features that are suitable for particular machine learning algorithms.</p>
    <p>One example is working with words in Natural Language Processing. Words are usually transformed to a list of numbers (embedded) before given as input to a neural network. The exact mapping between word and the list of numbers will be automatically learned.</p>
</td>
</tr>
<tr>
<td valign="top">Tensor (as in TensorFlow or PyTorch)</td>
<td>
    <p>A multidimensional array similar to <tt>numpy.array</tt></p>
    <p>Tensor is a term that is used in TensorFlow and PyTorch to indicate a multidimensional array. This may be a bit confusing, because the mathematical term tensor, actually has a different meaning - more like a function.</p>
    <p>Tensors are data structures that are used to store data. For example, a 1D tensor could store prices of houses, a 2D tensor could store an image, a 3D tensor could store multiple images etc.</p>
</td>
</tr>
<tr>
<td valign="top">Principal Component Analysis (PCA)</td>
<td>
    <p>An algorithm that removes less important data from a dataset.</p>
    <p>PCA (as any 'dimensionality reduction' algorithms) helps to reduce the storage space, to improve the performance of the models, and, to ease the data visualization.</p>
    <p>Technically, it's a statistical procedure that identifies and sorts a small number of uncorrelated variables, called principal components, in such a way that the first one has the most scattered data. So if we want to reduce from <tt>n</tt> to <tt>k</tt> dimensions, we keep the <tt>k</tt>'s first principal components. But the lower is <tt>k</tt> the greater is the information loss.</p>
</td>
</tr>
<tr>
<td valign="top">Kernel (function)</td>
<td>
    <p>A function that helps to separate datasets that can't be separated with a classic linear approach.</p>
    <p>A kernel function implicitly finds a higher dimensional space in which a non linearly separable dataset can be easily separated, then project the separation back to the original dataset space.</p>
    <p>Technically, a kernel function allows making complex non-linear classifiers using any learning algorithm that can be expressed solely in terms of dot products between two vectors.</p>
</td>
</tr>
<tr>
<td valign="top">Parameters</td>
<td>
    <p>The model parameters are the internal variables of the model that will be updated during the training phase, for example, in the case of neural networks, the weights or biases of the network.</p>
    <p>In some contexts, it is usual to describe a model by its number of parameters.</p>
</td>
</tr>
<tr>
<td valign="top">Hyperparameters</td>
<td>
    <p>Hyperparameters specify the model's architecture and how it will be trained. Therefore, these hyperparameters are not learned during training phase. In the case of neural networks, some common hyperparameters are:</p>
    <ul>
        <li>Learning rate</li>
        <li>Batch size</li>
        <li>Number of epochs to train the model</li>
        <li>Number of hidden layers</li>
        <li>Number of neurons in each layer</li>
        <li>Activations functions</li>
    </ul>
</td>
</tr>
<tr>
<td valign="top">Loss Function</td>
<td>
    <p>Function that is used to evaluate the performance of a model and guide the training process.</p>
    <p>Loss Functions (aka Cost Functions) show the error between what value your model predicts and what the value actually is. Since these functions are generally differentiable (with some exceptions i.e. Hinge Loss), we can apply a Gradient Descent to find the least error. Some common ones are:</p>
    <p>For Regression Models:</p>
    <ul>
        <li>Mean Absolute Error (MAE)</li>
        <li>Mean Squared Error (MSE)</li>
        <li>Mean Squared Logarithmic Error (MSLE)</li>
    </ul>
    <p>For Classification Models:</p>
    <ul>
        <li>Binary Cross Entropy Loss</li>
        <li>Categorical Cross Entropy Loss</li>
    </ul>
</td>
</tr>
<tr>
<td valign="top">Synthetic Data</td>
<td>
    <p>Synthetic data is comprised of data that isn’t based on any real-world phenomena or events, rather it’s generated via a computer program. The primary purpose of a synthetic dataset is to be versatile and robust enough to be useful for the training of machine learning models.</p>
</td>
</tr>
<tr>
<td valign="top">Ensemble Methods</td>
<td>
    <p>Ensemble methods are meta-algorithms that combine several machine learning techniques into one predictive model in order to </p>
    <ul>
        <li>Decrease variance (Bagging) </li>
        <li>Bias (Boosting)</li>
        <li>Improve predictions (Stacking)</li>
    </ul>
</td>
</tr>
<tr>
<td valign="top">Discriminatory Threshold</td>
<td>
    <p>The discrimination threshold is just the cutoff imposed on the predicted probabilities for assigning observations to each class. If you have a classifier (probabilistic) your output is a probability (a number between 0 and 1), ideally you want to say that everything larger than 0.5 is part of one class and anything less than 0.5 is the other class.</p>
</td>
</tr>
<tr>
<td valign="top">Overfitting</td>
<td>
    <p>Overfitting occurs when your model learns the training data too well and incorporates details and noise specific to your dataset. You can tell a model is overfitting when it performs great on your training/validation set, but poorly on your test set (or new real-world data).</p>
</td>
</tr>
<tr>
<td valign="top">Underfitting</td>
<td>
    <p>Underfitting occurs when your model over-generalizes and fails to incorporate relevant variations in your data that would give your model more predictive power. You can tell a model is underfitting when it performs poorly on both training and test sets.</p>
</td>
</tr>
</tbody>
</table>

Machine Learning terms are one thing the math is another. Get some human language explanation of some confusing terms [here](math-terms.md).
