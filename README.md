# File-handling
A code about File handling in python
### File handling and Exception HAndling

try:
    file=open('example1.txt','r')
    content=file.read()
    a=b
    print(content)

except FileNotFoundError:
    print("The file does not exists")
except Exception as ex:
    print(ex)

finally:
    if 'file' in locals() or not file.closed():
        file.close()
        print('file close')
if 'file' in locals():
    print(True)
