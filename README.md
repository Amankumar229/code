# code
make_folder_in_C_drive


directory = "Aman_senvion_work"
  
# Parent Directory path
parent_dir = r"C:\Users\aman.kumar.ext\Aman_senvion"
  
# Path
path = os.path.join(parent_dir, directory)
  
# Create the directory
try:
    os.makedirs(path, exist_ok = True)
    print("Directory '%s' created successfully" % directory)
except OSError as error:
    print("Directory '%s' can not be created" % directory)
