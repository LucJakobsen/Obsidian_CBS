### Lecture 1


### Lecture 2
[[Variables (Python)]]
[[General Python Syntax]]
[[Python Operators]]
[[Built-in Functions (Python)]]
[[Data Collection in Python]]

### Lecture 3
[[Python Libraries]]
[[Descriptive Analytics (Python)]]

Converting Jupyter notebook to pdf using visual studio code command window:
``jupyter nbconvert --to pdf "document"

Needs to be installed via Pip first:
``%load_ext nb_black
- Will make the code prettier

Excercise 2:
i = 0, stands for index = 0


**Converting a table into a dataframe**:
``pd.DataFrame(data=x, columns=["Frequency"])

``df.reset_index(inplace=True)`` --> will reset the index so that the value is no longer considered the index

renaming columns:
``df.columns = ["value", "frequency"]


adding percentages to the frequency table:
``df["percentage"] = df["frequency"] / sum(df["frequency"])

For matplotlib, using axes will give us more control over e.g. the size of the graph as it is printed "on top" of the figure


- Check up on variable density


- check up on ``with`` statement