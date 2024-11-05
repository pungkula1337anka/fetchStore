# fetchStore
Fetch Store Information from Open Street Map.


# Setup and Usage

For usage with Home Assistant:

**1. Create Shell Command** 

    ```
    shell_command:
      fetchstore: >
        python3 fetchStore.py "{{ store | replace('\"', '') }}" "{{ location | replace('\"', '') if location | length > 0 else 'Paris, France' }}" "{{ radius | replace('\"', '') if radius | length > 0 else '3000' }}"
    ```

Please change the default City and Country f you want to be able to use the location optionally.


**2. Create the script**

In `/config` create a file named `fetchStore.py`.

```

```
