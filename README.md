## Split-our-Bill-App

#### Split billing is the division of a bill for service into two or more parts.
 #### Bills may be split to divide work between clients, payers or for reimbursement to different service providers for performing a shared service.
----
![img](https://github.com/marina-gu/split-our-bill/blob/main/split_bill.png)

----
### Stack

__To build the Split our Bill-App were used__

- HTML
- CSS
- JavaScript

```JavaScript
function  calculateAmount(e) {
    e.preventDefault();

    const bill = document.querySelector('#bill').value;
    const people = document.querySelector('#people').value;
    const tip = document.querySelector('#tip').value;
    if (bill=== "" || people === "" || people < 1) {
        Swal.fire({
            icon: 'error',
            title: 'Error!',
            text: 'Please enter your information!'
        })
    }

    let amountPerPerson = bill/people;
    let tipPerPerson =(bill*tip) /people;
    let totalSum = amountPerPerson + tipPerPerson;
```
  ----

### Open [link](https://split-ourbill-project.glitch.me/) to view it in your browser.
----

![gif](https://github.com/marina-gu/split-our-bill/blob/main/IMG_1379.gif)

  


