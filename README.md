Name(s):
    - Kenneth Doan

Python Version: 3.9.4

Instructions:
    1. Extract worm.py from the .zip file
    2. Using your OS's command-line / terminal, navigate to the main directory that contains the extracted worm.py
    3. Type "python3 worm.py" into the command-line / terminal and press Enter.

Extra Credit Done:
    - None

Additional Information:
    - I had to use pynetinfo from "pip install git+https://github.com/9b/pynetinfo", not from the default pip installation from https://github.com/sassanp/pynetinfo
        - I don't know the exact differences between Python2 and Python3, so trying to get the Pynetinfo module from https://github.com/sassanp/pynetinfo to work was too time-consuming.
            - Issues with the module from sassanp involve, at least:
                - conflicting types for ‘initnetinfo’
                    - solved with https://stackoverflow.com/questions/10509400/difference-between-pymodinit-func-and-pymodule-create
                - Python module import error: "undefined symbol: Py_InitModule3" (Py_InitModule ())
                    - solved with https://stackoverflow.com/questions/43621948/c-python-module-import-error-undefined-symbol-py-initmodule3-py-initmodu
                - ImportError: dynamic module does not define module export function
                    - unable to resolve
                    - tried everything from https://stackoverflow.com/questions/55277328/unable-to-solve-importerror-dynamic-module-does-not-define-module-export-funct

    - As a head's up, I installed (regular) nmap--from the default installation of "pip3 install nmap"--to troubleshoot the PortScanner's scan function and check on the status of each VM's port 22. I don't know if having python-nmap and regular nmap together causes issues or messes with the intended results of this assignment.

    - Tested on 3 instances of a Lubuntu 21.04 Hirsute Hippo VM from osboxes