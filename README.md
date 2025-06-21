# Calc.sh
Calculator on shell
while [ true ]
do
       echo "1. Addition"
       echo "2. substraction"
       echo "3. Exit"

      read -p "enter your choice:" choice

      case $choice in
               1) read -p "Enter first number:" num1
                  read -p "Enter second number:" num2
                  expr $num1 + $num2
                  ;;
               2) echo "sub"
                  ;;
               3) break
                  ;;
               *) echo "valid chioce:"
                  ;;
      esac
done
