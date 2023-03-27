<!-- Autogenerated by docgen; don't manually edit -->
### `RunSQL`

Run a SQL statement and return a list of tensors in private status  

**Inputs:**  

No input parameter.


**Outputs:**  

1. `Out`(variadic, T): Result tensors of the SQL statement.



**Attributes:**  

1. `sql`: SQL statement

1. `table_refs`: tables referenced by query






**TensorStatus(ShareType) Constraints:**

1. `T`: private



### `Publish`

This operator publishes the DAG results.  

**Inputs:**  

1. `In`(variadic, T1): Tensors to be published.


**Outputs:**  

1. `Out`(variadic, T2): Result tensors of the publish op. Tensors are in TensorOption VALUE.






**TensorStatus(ShareType) Constraints:**

1. `T1`: public,private

1. `T2`: unknown



### `Less`

Out = Left `Less` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `LessEqual`

Out = Left `LessEqual` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Greater`

Out = Left `Greater` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `GreaterEqual`

Out = Left `GreaterEqual` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Equal`

Out = Left `Equal` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `NotEqual`

Out = Left `NotEqual` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `LogicalAnd`

Out = Left `LogicalAnd` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `LogicalOr`

Out = Left `LogicalOr` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Add`

Out = Left `Add` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Minus`

Out = Left `Minus` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Mul`

Out = Left `Mul` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Div`

Out = Left `Div` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `IntDiv`

Out = Left `IntDiv` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `Mod`

Out = Left `Mod` Right  

**Inputs:**  

1. `Left`(variadic, T): First operand.

1. `Right`(variadic, T1): Second operand.


**Outputs:**  

1. `Out`(variadic, T2): Output Tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: public,private,secret

1. `T2`: private,secret



### `MakePublic`

Convert In tensor from share/private status to public status.  

**Inputs:**  

1. `In`(variadic, T1): Input tensors.


**Outputs:**  

1. `Out`(variadic, T2): Output tensors.






**TensorStatus(ShareType) Constraints:**

1. `T1`: private,secret

1. `T2`: public



### `MakePrivate`

Convert In tensor from share status to private status.  

**Inputs:**  

1. `In`(variadic, T1): Input tensors.


**Outputs:**  

1. `Out`(variadic, T2): Output tensors.



**Attributes:**  

1. `reveal_to`: List of parties to see the private data. If it is revealed to one party only, the other party also needs to run the op, but does not have an output. Only the reveal_to party gets the output.






**TensorStatus(ShareType) Constraints:**

1. `T1`: secret

1. `T2`: private



### `MakeShare`

Convert In tensor from private status to share status.  

**Inputs:**  

1. `In`(variadic, T1): Input tensors.


**Outputs:**  

1. `Out`(variadic, T2): Output tensors.






**TensorStatus(ShareType) Constraints:**

1. `T1`: private

1. `T2`: secret



### `Join`

Definition: Create Join Index based on EQ-Join, return result's corresponding rows index in the original input.
Example:

```python
// inner join example
Left = {4,4,3,2,1} // shape:[M=5]
Right = {1,3,4,5} // shape: [N=4]
LeftJoinIndex = {4,2,0,1}  // shape:[K=4], rows after applied filter eq-join-list={1,3,4,4}
RightJoinIndex = {0,1,2,2} // shape:[K=4], rows after applied filter eq-join-list={1,3,4,4}
```
  

**Inputs:**  

1. `Left`(single, T1): Left vector(shape [M][1])

1. `Right`(single, T1): Right vector(shape [N][1])


**Outputs:**  

1. `LeftJoinIndex`(single, T2): Joined rows index for left vector(shape [K][1])

1. `RightJoinIndex`(single, T2): Joined rows index for right vector(shape [K][1])



**Attributes:**  

1. `input_party_codes`: List of parties the inputs belong to([PartyCodeLeft, PartyCodeRight]).

1. `join_type`: Int64. 0: inner join;






**Default Attribute Values:**

1. `join_type`: 0




**TensorStatus(ShareType) Constraints:**

1. `T1`: private

1. `T2`: private



### `FilterByIndex`

Definition: Filter by rows index.
Example:

```python
RowsIndexFilter = {3,1,0}
Data = [{"a", "b", "c", "d"}, {0, 1, 2, 3}]
Out = [{"d", "b", "a"}, {3, 1, 0}]
```
  

**Inputs:**  

1. `RowsIndexFilter`(single, T): Rows index filter vector(shape [K][1]).

1. `Data`(variadic, T): Input data tensor(shape [M][N]).


**Outputs:**  

1. `Out`(variadic, T): Output data tensor(shape [X][N]).






**TensorStatus(ShareType) Constraints:**

1. `T`: private



### `Copy`

Definition: Copy source tensor "In" to new tensor "Out" on target party  

**Inputs:**  

1. `In`(single, T1): source tensor


**Outputs:**  

1. `Out`(single, T1): target tensor



**Attributes:**  

1. `input_party_codes`: Input tensor `In` belongs to

1. `output_party_codes`: Output tensor `Out` belongs to






**TensorStatus(ShareType) Constraints:**

1. `T1`: private



### `Filter`

Given a boolean tensor Filter (its shape is [M]), and a number of tensors In
(variadic, each tensor's shape must be [M]), for i in [0, M-1], keep the In tensors' element if and only if Filter[i]
is True, output the filter result tensors Out (variadic). Example:

```python
Filter = {True, False, False, True, False}
In = {a, b, c, d, e}
Out = {a, d}
```
  

**Inputs:**  

1. `Filter`(single, T1): Filter tensor.

1. `In`(variadic, T): Tensors to be filtered.


**Outputs:**  

1. `Out`(variadic, T): Output tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret

1. `T1`: public,private



### `Constant`

Definition: Make constant from attribute.
Example:

```python
scalar = [{"a", "b", "c"}]
to_status = 0
Out = [{"a", "b", "c"}]
```
  

**Inputs:**  

No input parameter.


**Outputs:**  

1. `Out`(single, T): output tensor(shape [M]) from constant.



**Attributes:**  

1. `scalar`: scalar attribute(with shape [M])

1. `to_status`: int64. to status, 0: to private, 1: to public.






**Default Attribute Values:**

1. `to_status`: 0




**TensorStatus(ShareType) Constraints:**

1. `T`: public,private



### `DumpFile`

Definition: Dump the input tensor. Note: This op will change the affected rows in the session  

**Inputs:**  

1. `In`(variadic, T): Tensors to be dumped.


**Outputs:**  

1. `Out`(variadic, T): Tensors have been dumped.



**Attributes:**  

1. `file_path`: String. Absolute file path to dump the tensors.

1. `deliminator`: String. Column deliminator, e.g. comma `,`






**TensorStatus(ShareType) Constraints:**

1. `T`: private



### `In`

Definition: Given an input tensor Left (its shape is [M]), and another input tensor Right (its shape is [N]),
check whether Left's element exists in Right's elements and output a boolean tensor Out (its shape is [M]). Left and Right must be the same type.
Example:

```python
Left = {a, b, c, d}
Right = {b, d, e, f, g, h}
Out = {False, True, False, True}
```
  

**Inputs:**  

1. `Left`(single, T): First operand.

1. `Right`(single, T1): Second operand.


**Outputs:**  

1. `Out`(single, T): Output Tensor.



**Attributes:**  

1. `algorithm`: Int64. Algorithm to use for the op. 1: PSI

1. `input_party_codes`: List of parties the inputs belong to. This attribute is required if algorithm = PSI.

1. `reveal_to`: A party can see the result. This attribute is required if algorithm = PSI.






**Default Attribute Values:**

1. `algorithm`: 0




**TensorStatus(ShareType) Constraints:**

1. `T`: private

1. `T1`: private



### `ReduceSum`

Definition: Given an input tensor In, return the sum of input tensor's elements.
Example:

```python
In = {1, 2, 3, 4, 5, 6}
Out = {21}
```
  

**Inputs:**  

1. `In`(single, T): Tensor to be summed (shape [M]).


**Outputs:**  

1. `Out`(single, T): The summed Tensor (shape [1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret



### `ReduceMax`

Definition: Given a input tensor In, return the max of input tensor's elements.
Example:

```python
In = {1, 2, 3, 4, 5, 6}
Out = {6}
```
  

**Inputs:**  

1. `In`(single, T): Tensor to be maxed (shape [M]).


**Outputs:**  

1. `Out`(single, T): The maxed Tensor (shape [1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret



### `ReduceMin`

Definition: Given a input tensor In, return the min of input tensor's elements.
Example:

```python
In = {1, 2, 3, 4, 5, 6}
Out = {1}
```
  

**Inputs:**  

1. `In`(single, T): Tensor to be mined (shape [M]).


**Outputs:**  

1. `Out`(single, T): The mined Tensor (shape [1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret



### `ReduceAvg`

Definition: Given a input tensor In, return the average of input tensor's elements.
Example:

```python
In = {1, 2, 3, 4, 5}
Out = {3}

In = {1, 2, 3, 4}
Out = {2.5}
```
  

**Inputs:**  

1. `In`(single, T): Tensor to be reduced (shape [M]).


**Outputs:**  

1. `Out`(single, T): The average Tensor (shape [1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret



### `Shape`

Definition: Given tensors In, return shapes of each tensor. Axis starts from 0. If axis is set, dimensions of each shape are returned. If axis is not set(default -1), shapes are returned.
Example:

```python
In = {{1, 2}, {2, 3}, {4, 3, 3}} # {1, 2} here is a column vector
Out = {{2, 1}, {2, 1}, {3, 1}}
```
  

**Inputs:**  

1. `In`(variadic, T): Input Tensors


**Outputs:**  

1. `Out`(variadic, T1): Shape Tensors



**Attributes:**  

1. `axis`: Int. Specific dimension of the shape.






**Default Attribute Values:**

1. `axis`: -1




**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret

1. `T1`: private



### `Unique`

Definition: Unique of Key tensor.
Example:

```python
Key = {"a", "b", "a", "d"}
UniqueKey = {"a", "b", "d"}
```
  

**Inputs:**  

1. `Key`(single, T): Input key tensors(shape [M][1]).


**Outputs:**  

1. `UniqueKey`(single, T): Output unique key tensor(shape [K][1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: private



### `Sort`

Definition: sort `In` using `Key`.
Example:

```python
Key = {3, 1, 2, 4}
In = [{3, 1, 2, 4}, {1, 2, 3, 4}, {9, 8, 7, 6}]
Out = [{1, 2, 3, 4}, {2, 3, 1, 4}, {8, 7, 9, 6}]
```
  

**Inputs:**  

1. `Key`(variadic, T): Sort Key(shape [M][1]).

1. `In`(variadic, T): Sort Value(shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Sorted Value(shape [M][1])



**Attributes:**  

1. `reverse`: Bool. If True, the sorted tensor in descending order.






**Default Attribute Values:**

1. `reverse`: false




**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret



### `ObliviousGroupMark`

Definition: generate end of group indicator `Group` based on `Key`. The operator calculates Group[i] = not_eq(Key[i+1], Key[i]).
Example:

```python
Key = [{0, 0, 0, 1}, {0, 1, 1, 1}]
Group = {1, 0, 1, 1}

Key = [{0, 0, 1, 2, 2}]
Group = {0, 1, 1, 0, 1}
```
  

**Inputs:**  

1. `Key`(variadic, T): Pre-sorted group keys (shape [M][1]).


**Outputs:**  

1. `Group`(single, T): End of group indicator(shape [M][1]). Element 1 means the row is the last element of the group, 0 is not.






**TensorStatus(ShareType) Constraints:**

1. `T`: private,secret



### `ObliviousGroupSum`

Definition: partially aggregate `In` according to end of group indicator.
Example:

```python
Group = {1, 0, 0, 1, 1}
In = [{1, 3, 2, 4, 0}, {9, 8, 7, 6, 5}]
Out = [{1, 3, 5, 9, 0}, {9, 8, 15, 21, 5}]
```
  

**Inputs:**  

1. `Group`(single, T): End of group indicator(shape [M][1]). Element 1 means the row is the last element of the group, 0 is not.

1. `In`(variadic, T): Values to be aggregated (shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Partially aggregated values (shape [M][1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: secret



### `ObliviousGroupCount`

Definition: partially aggregate `In` according to end of group indicator.
Example:

```python
Group = {1, 0, 0, 1, 1}
In = [{1, 3, 2, 4, 0}, {9, 8, 7, 6, 5}]
Out = [{1, 1, 2, 3, 1}, {1, 1, 2, 3, 1}]
```
  

**Inputs:**  

1. `Group`(single, T): End of group indicator(shape [M][1]). Element 1 means the row is the last element of the group, 0 is not.

1. `In`(variadic, T): Values to be aggregated (shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Partially aggregated values (shape [M][1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: secret



### `ObliviousGroupMax`

Definition: partially aggregate `In` according to end of group indicator.
Example:

```python
Group = {1, 0, 0, 1, 1}
In = [{1, 3, 2, 4, 0}, {9, 8, 7, 6, 5}]
Out = [{1, 3, 3, 4, 0}, {9, 8, 8, 8, 5}]
```
  

**Inputs:**  

1. `Group`(single, T): End of group indicator(shape [M][1]). Element 1 means the row is the last element of the group, 0 is not.

1. `In`(variadic, T): Values to be aggregated (shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Partially aggregated values (shape [M][1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: secret



### `ObliviousGroupMin`

Definition: partially aggregate `In` according to end of group indicator.
Example:

```python
Group = {1, 0, 0, 1, 1}
In = [{1, 3, 2, 4, 0}, {9, 8, 7, 6, 5}]
Out = [{1, 3, 2, 2, 0}, {9, 8, 7, 6, 5}]
```
  

**Inputs:**  

1. `Group`(single, T): End of group indicator(shape [M][1]). Element 1 means the row is the last element of the group, 0 is not.

1. `In`(variadic, T): Values to be aggregated (shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Partially aggregated values (shape [M][1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: secret



### `ObliviousGroupAvg`

Definition: partially aggregate `In` according to end of group indicator.
Example:

```python
Group = {1, 0, 0, 1, 1}
In = [{1, 3, 2, 4, 0}, {9, 8, 7, 6, 5}]
Out = [{1, 3, 2.5, 3, 0}, {9, 8, 7.5, 7, 5}]
```
  

**Inputs:**  

1. `Group`(single, T): End of group indicator(shape [M][1]). Element 1 means the row is the last element of the group, 0 is not.

1. `In`(variadic, T): Values to be aggregated (shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Partially aggregated values (shape [M][1]).






**TensorStatus(ShareType) Constraints:**

1. `T`: secret



### `Shuffle`

Definition: Shuffle `In`.
Example:

```python
In = [{1, 2, 3, 4}, {9, 8, 7, 6}]
Out = [{4, 3, 2, 1}, {6, 7, 8, 9}]
```
  

**Inputs:**  

1. `In`(variadic, T): Input Value(shape [M][1]).


**Outputs:**  

1. `Out`(variadic, T): Output Value(shape [M][1])






**TensorStatus(ShareType) Constraints:**

1. `T`: secret



### `BroadcastTo`

Definition: Broadcast Input tensor `In` to the same shape as `ShapeRefTensor`. 
Example:
```Python
In = [1]
ShapeRefTensor = [a, b, c]
# ShapeRefTensor's shape is (3, 1), broadcast In to shape (3, 1)
Out = BroadcastTo(In, ShapeRefTensor) = [1, 1, 1]
```
  

**Inputs:**  

1. `In`(variadic, T): Input tensor

1. `ShapeRefTensor`(single, T1): Shape reference tensor


**Outputs:**  

1. `Out`(variadic, T2): Result tensor






**TensorStatus(ShareType) Constraints:**

1. `T`: public

1. `T1`: public,private,secret

1. `T2`: public,private



### `Not`

Out = Not In  

**Inputs:**  

1. `In`(single, T): Input tensor.


**Outputs:**  

1. `Out`(single, T): Output tensor.






**TensorStatus(ShareType) Constraints:**

1. `T`: public,private,secret



### `Concat`

Definition: Given a number of tensors In (variadic, each tensor's shape must be the same except for the axis), concat the In tensors along the axis.
Example:

```python
In = {{1, 2}, {2, 3, 4}, {3, 4, 5, 6}}
Out = {1, 2, 2, 3, 4, 3, 4, 5, 6}
```
  

**Inputs:**  

1. `In`(variadic, T): Tensors to be concat.


**Outputs:**  

1. `Out`(single, T): Concated Tensor.



**Attributes:**  

1. `axis`: Int. Dimension along which to concatenate.






**Default Attribute Values:**

1. `axis`: 0




**TensorStatus(ShareType) Constraints:**

1. `T`: secret



