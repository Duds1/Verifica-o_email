def validar_email(email):
    if "@" in email and not email.startswith("@") and not email.endswith("@") and " " not in email:
        partes = email.split("@")
        if len(partes) == 2 and "." in partes[1]:
            print("E-mail válido")
            return
    print("E-mail inválido")


email = input()
validar_email(email)
