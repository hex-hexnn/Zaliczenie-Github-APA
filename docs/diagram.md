graph TD
    A([START]) --> B[Strona główna]
    B --> C{Użytkownik zalogowany?}

    C -- NIE --> D[Rejestracja / Login]
    D --> E[Walidacja danych]
    E --> F{Błąd?}
    F -- TAK --> G[Komunikat błędu]
    G --> H[Powrót do formularza]

    C -- TAK --> I[Panel użytkownika]
    I --> J[Wybór akcji]
    J --> K[Dodaj transakcję]
    K --> L[Formularz transakcji]
    L --> M[Walidacja danych]
    M --> N{Błąd?}
    N -- TAK --> O((...))