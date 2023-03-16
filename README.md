# Lab-5_202001178

## Name: Rudra Gohel
## ID: 202001178

**Aim**: Select the tool of your choice. Select a git repository, use the selected tool and analyze the files from the selected repository. Submit the tool output and understanding of the errors.

**Tool Used**: mypy

Installation 

![image](https://user-images.githubusercontent.com/107960916/225580915-f4e31492-de5e-495a-bbaa-aced78239cf7.png)

Mypy is already installed on the system.

**Repository analyzed**: https://github.com/Rudragohel/woc4.0-eventmanager-Rudra-Gohel

**Analysis**: 

**File 1**: pysc1.py (link: https://github.com/Rudragohel/woc4.0-eventmanager-Rudra-Gohel/blob/main/Python_Scripts/PyScript-1/pysc1.py)

![image](https://user-images.githubusercontent.com/107960916/225574135-f57d3ed1-3f23-41c9-ac53-ed8934139d79.png)

Errors detected using mypy:

Total 6 errors are detected.
First 4 errors are import errors. These indicate that in order to run this python file, it requires some libraries which are not installed yet. These uninstalled libraries are "cricketstats", "networkx", "matplotlib.pyplot", "matplotlib". 

5th error is of type operator. It indicates that operator + is unsupported for ("int" and "object") together. This tells int and object datatype cannot be added together. 

6th error is of type call-overload. It indicates that function "__getitem__" has no other variant that inputs list of object as input.

However errors 5 and 6 are due to not including above mentioned "networkx" library. If we install that library, these error 5 and 6 will go away on its own. 

**File 2**: pysc2.py (link: https://github.com/Rudragohel/woc4.0-eventmanager-Rudra-Gohel/blob/main/Python_Scripts/PyScript-2/pysc2.py)

![image](https://user-images.githubusercontent.com/107960916/225577311-a4a696f8-2655-4e77-8dd7-c39402fd3d47.png)

Errors detected using mypy:

Total 4 errors are detected.

All are import errors. File requires "cricketstats", "chess", "chess.pgn", "stockfish" libraries to execute correctly. 

**Conclusion**

All errors are detected correctly.
However some errors are redundant. For example in file1, if we import "networkx" library other 2 errors are solved automatically. That is solving 1 error(error number 2), other 2 errors(error 5 and error 6) are solved on their own. Hence these 2 errors are redundant. 

