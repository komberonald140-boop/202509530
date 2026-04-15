#WORKFLOW
┌───────────────┐
        │     START     │
        └──────┬────────┘
               │
               ▼
        ┌───────────────┐
        │   Input n     │
        └──────┬────────┘
               │
               ▼
        ┌───────────────┐
        │ a = 0, b = 1  │
        │ i = 0         │
        └──────┬────────┘
               │
               ▼
        ┌───────────────┐
        │  i < n ?      │
        └──────┬────────┘
          Yes  │   No
               │
               ▼
        ┌───────────────┐
        │ Print a       │
        └──────┬────────┘
               │
               ▼
        ┌───────────────┐
        │ temp = a + b  │
        └──────┬────────┘
               │
               ▼
        ┌───────────────┐
        │ a = b         │
        │ b = temp      │
        └──────┬────────┘
               │
               ▼
        ┌───────────────┐
        │ i = i + 1     │
        └──────┬────────┘
               │
               └───────↺ (back to i < n)

               ▼
        ┌───────────────┐
        │     END       │
        └───────────────┘
        #PSEUDOCODE
        FUNCTION Fibonacci(n)

    IF n == 0 THEN
        RETURN 0

    ELSE IF n == 1 THEN
        RETURN 1

    ELSE
        RETURN Fibonacci(n - 1) + Fibonacci(n - 2)

    END IF

END FUNCTION
#PYTHONCODE
def fibonacci(n):
    if n == 0:
        return 0
    elif n == 1:
        return 1
    else:
        return fibonacci(n-1) + fibonacci(n-2)
