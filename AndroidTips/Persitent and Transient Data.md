* Title : What is difference between persistent data and transient data?
* Tip-number : 02
* Tip-username : Bhagyasree
* Tip-Description : What is difference between persistent data and transient data, give one example. Also tell me which activity life cycle function I need to use to save them.

---

- [Differences] (#What is difference?)
- [Example] (#How to use?)
- [Life cycle] (#Function to use?)

---

## <a name="What is difference?"> Differences </a>

Persistent data is permanent data. A persistent object is an instance of a class in the domain model that represents some information extracted from the database. Transient data is logical data. A transient object is an instance of a class in the domain model, which is created in memory

## <a name="How to use?"> Example </a>

### Persistent Data
   - We use in database tables
   
### Transient Data
   - Logical data we use in programming language

## <a name="Function to use?"> Life cycle </a>

#### Life cycle to save

```
       @Override
       public void onSaveInstanceState(Bundle savedInstanceState) {
       super.onSaveInstanceState(savedInstanceState);
       }
```

#### Life cycle to Retrieve
```
       @Override
       public void onRestoreInstanceState(Bundle savedInstanceState) {
       super.onRestoreInstanceState(savedInstanceState);
```
