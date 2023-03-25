<html>
<head>
    <title>user Form</title>
</head>
<body>
    <h1>user Form</h1>
    <form id="user-form">
    <label for="name".Name:</label>
    <input type="text" id="name name="name required>
    <br>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>
    <br>
    <label for="phone">phone:</label>
    <input type="tel" id="phone" name="phone" required>
    <br>
    <button type="submit">submit</button></form>
    <script>
    const form = document.getElementById('user-form');
    form.addEventListner('submit',('event')=> {
        event.preventDefault();
        const name = document.getelementById('name').value;
        const email = document.getelementById('email').value;
        const phone = document.getelementById('phone').value;
        const url = 'https://example.com/api/user?name=${name}&email=${email}&phone=${phone};
        fetch(url, { method; 'GET' })
        .then(response => {
         if(response.ok) {
           return response.json();
           }else{
            throw new eroe('user not found');
            }
            })
            .then(data =>{
            alert('user not found');
            })
            .catch(error => {
            console.error(error);
            
           const createuserurl ='https://example.com/api/user';
           const userdata ={ name,email,phone};
           fetch(createuserurl, {
           headers: {
            'content-type':application/json'
            },
            
           
            
   
    
