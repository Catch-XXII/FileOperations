import os

path = os.getcwd()
print('Your current directory is %s' % path)
folder = input("Enter a folder name: ")
directory = '{}/{}'.format(path, folder)
if os.path.exists(folder):
    print("Folder name already exists!...\nPlease specify another name.")
else:
    try:
        os.mkdir(directory)
    except:
        print("Creation of the directory %s failed" % path)
    else:
        print("Successfully created the folder %s " % folder + "under " + directory)
# Change the directory and create a txt file under that folder.
os.chdir(directory)
print("You're now on directory: " + os.getcwd())
filename = input("Please enter a file name: ")
filename = filename + '.txt'
with open(filename, "w+") as f:
    for i in range(10):
        f.write("This is line %d\r\n" % i)
