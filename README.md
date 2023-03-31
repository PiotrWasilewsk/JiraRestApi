# JiraRestApi
Repozytorium "JiraRestApi" jest zestawem testów dla aplikacji JIRA uruchamianej lokalnie na hoście: **http://localhost:8080/**. Na podstawie dokumentacji API sporządziłem kolekcję w programie Postman o takiej samej nazwie jak repozytorium. Kolekcja "JiraRestApi" zawiera następujace request-y:
- Autenthication, 
- GetAllProjects, 
- CreateNewProject,
- GetAllProcectsAfterCreated,
- GetSingleProject,
- DeleteProject,
- GetSingleProjectAfterDelete.

Na potrzeby powyższych request-ów opracowałem zestawy testów, które swoim zakresem, obejmuja jak najszersze spektrum wystąpienia błędów, zarówno jeśli chodzi o kody statusów wysyłanych z serwera, jak i niektóre funkcje które umożliwia aplikacja oraz poprawnie sformatowane ciała odpowiedzi.
Kolekcja "JiraRestApi" zawiera "szczęśliwą ścieżkę" reprodukcyjną.
Do przeprowadzenia powyższych testów potrzeba ustawić serwer Jira na naszym lokalnym systemie. Aby to zrobić należy podjąć następujące kroki:
- Pobrać ze strony **https://www.atlassian.com/software/jira/update** Jira software,
- Uruchomić instalatora,
- Na tablicy "Welcome to the Jira software installation wizard" kliknąć w przycisk "Next",
- Na kolejnej tablicy zaznaczyć opcję "Express install" i kliknąć w przycisk "Next",
- Na tablicy "Windows security alert" zaznaczyć oba checkbox-y i kliknąć w przycisk "Allow access",
- Na tablicy "Installation summary" kliknąć w przycisk "Install",
- Na tablicy "Installation of Jira software (ver) is complete" kliknąć przycisk "Next",
- Na kolejnej tablicy kliknąć przycisk "Finish". W przegladarce uruchamia sie serwer,
- Po uruchomieniu serwera wybrać "Set it up for me" i kliknąć w przycisk "Continue to MyAtlassian",
- Następnie w zależności należy się zalogowoć lub utworzyć konto,
- W kolejnym kroku potwierdzić licencję wybierając opcję "Jira software data center",
- Następnie ustawićkonto administratora należy uzupełnić pola "email", "username" oraz "password", kliknąć przycisk "Next",
- Instalacja zostaje zakończona.

Należy pamiętać, że przy każdym ponownym włączeniu komputera należy uruchomić serwer localhost8080. Można to zrobić np wciskająć na klawiaturze znaczek "windows", wpisać z klawiatury "Jira" i kliknąć w "Start Jira Server"
