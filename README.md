# Sistema de Importacao Treinamento
This system will automate some manual and repetitive tasks, so that it can be performed quickly and free of human errors. 

## Stakeholder context
My team is responsible for setting up work equipment for new employees. When the training takes place, the responsible department sends us a database in Excel 
Spreadsheet format with the information of the new employees, so we start the following process:

- Download the worksheet "ListaTreinamento.xlsx" from the email, it will contain employee data such as name, date of birth and others
- Format cell values, removing spaces before the word, special characters like "@*-_"
- Create a DOCX file to print labels for each employee's equipment
- Convert the XLSX file to a JSON, so that it can be sent to the server in a registration request in the system
- Email the formatted spreadsheet and labels to the other collaborators on the team

After all this process we can finally start preparing the equipment. We have a time-consuming routine that may have human errors, so there is a need for a system 
that automates this process.

## Software Architecture
The program needs to be responsible and easy to use, automating the stakeholder's processes. The Architecture is documented in my 
[Figjam file (pt-br)](https://www.figma.com/file/9nKZcNv6uewaRSzuFtdvet/Automatiza%C3%A7%C3%A3o-Lista-de-Treinamento?node-id=0-1&t=HfGqiX82cFKVv6l3-0)

To automate the process and ensure responsivity, it will be necessary to have some requirements:

- Character formatting algorithm for name and CPF patterns
- xlsx file conversion to JSON
- Conversion to a DOCX file in special format for printing
- Request WebService for data registration
- Automatic email sending with personalized message
