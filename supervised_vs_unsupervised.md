# Supervised vs. Unsupervised Machine Learning

---

**Machine Learning**:
- "Field of study that gives computers the ability to learn without being explicitly programmed."

In general the more opportunities you give the machine chances to try; the better the model will perform

**Machine Learning Algorithms**
- Supervised Learning
    - Used most in real world applications
    - Rapid Advancements
- Unsupervised Learning
- Recommender systems
- Reinforcement learning

Practical advice for applying learning algorithms

### Supervised Learning

---

- algorithms that learn x --> Y aka input --> mappings
- give your learning algorithms examples to learn from that has the correct answer; correct label y of input x
- learning algo learns to take just x and return a reasonable y

**Regression**: Housing price prediction

![alt text](/images/regression.png)

- an algorithm to systematically choose the most appropriate line or curve to fit this data
- predict a number from infinitely many possible outputs

**Classification Algorithm**
- Breast cancer detection
- malignant or benign
- x = size (diameter in cm) y = diagnosis (0 or 1)
- Two possible outputs makes this classification
- It is possilbe to have more than two output classifications
- Multiple types of cancer diagnosis if malignant
- malignant type 1 
- malignatn type 2
- output classes and output categories are often used interchangeably 
- classification algo predict categores
- small number of possible outputs vs. regression (infinitely many possible outputs)
- Two or more inputs:
    - Age and tumor size
    - decide how to fit a boundary line to this data

### Unsupervised Learning 

--- 

- Given data that isn't associated with any output labels y
- given age and tumor size but not whether the tumor is benign or malignant
- Job is to find some structure or something interesting in unlabeled data
- might decide that the data belongs into two different clusters
    - **clustering algorithm**
    - used in Google news
        - groups related news together
    
- Clustering: DNA microarray
    - measure how much certain genes are expressed in individuals
    - clustering algorithms to group individuals

- Clustering: Grouping Customers
    - Different market segments

**Unsupervised Learning**: 
- Data only comes with inputs x, but not output labels y
- Algorithm has to find *structure* in the data
- **Clustering**
    - group similar data points together
- **Anomaly Detection**
    - Find unusual data points
- **Dimensionality reduction**
    - compress data using fewer numbers


