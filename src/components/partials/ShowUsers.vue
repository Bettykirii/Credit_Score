// vue-template.vue


<template functional>
<div style="overflow-x:auto;">    
  <table class="table table-striped table-bordered">
            <thead>
                <tr>

                <th>Name</th>
                <th>Interest</th>
                <th>Balance</th>
                <th>AnnualInterestRate</th>
                <th>MonthlyPaymentRate</th>
                <th>Age</th>
                <th>Delinquency</th>
                <th>DebtRatio</th>
                <th>NumberOfOpenCreditLinesAndLoans</th>
                <th>NumberOfTime30To59DaysPastDueNotWorse</th>
                <th>NumberOfTime90DaysLate</th>
                <th>NumberOfRealEstateLoanAndLines</th>
                <th>NumberOfTime60To89DaysPastDueNotWorse</th>
                <th>NumberOfDependants</th>

         
           
                </tr>
            </thead>
            <tbody>
                <tr v-for="user in usersList" :key="user.id">
                    <td>{{user.id}} {{user.name}}</td>
                    <td>{{user.interest}}</td>
                <td>{{user.balance}}</td>
                <td>{{user.annualInterestRate}}</td>
                <td>{{user.monthlyPaymentRate}}</td>
                <td>{{user.age}}</td>
                <td>{{user.delinquency}}</td>
                <td>{{user.debtRatio}}</td>
                <td>{{user.numberOfOpenCreditLinesAndLoans}}</td>
                <td>{{user.numberOfTime30To59DaysPastDueNotWorse}}</td>
                <td>{{user.numberOfTime90DaysLate}}</td>
                <td>{{user.numberOfRealEstateLoanAndLines
                  }}</td>
                <td>{{user.numberOfTime60To89DaysPastDueNotWorse}}</td>
                <td>{{user.numberOfDependants}}</td>

                </tr>
            </tbody>
        </table>

    
  </div>
</template>

<script>
export default {
  data() {
    return {
      usersList: []
    };
  },
 mounted() {
    const proxyurl = "https://cors-anywhere.herokuapp.com/";
     const url = "https://rose-credit-card-api.herokuapp.com/creditCard";
   fetch(proxyurl + url).then((res) => {
          return res.json();
      }).then((users) => {
          this.usersList.push(...users);
      }).catch(() => console.log("Can’t access " + url + " response. Blocked by browser?"))
      
  }
};
</script>

<style>

 table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
 
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 4px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}
</style>