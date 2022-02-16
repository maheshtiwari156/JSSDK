<html>
    <head>
        <script language="JavaScript" type="text/javascript" src="/js/jquery-1.2.6.min.js"></script>
        <script language="JavaScript" type="text/javascript" src="/js/jquery-ui-personalized-1.5.2.packed.js"></script>
        <script language="JavaScript" type="text/javascript" src="/js/sprinkle.js"></script>
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
        <script>$(document).ready(function(){
            console.log("asdad");
            $.ajax({
            url : 'https://www.yammer.com/api/v1/users/by_email.json?email=mahesh@cnx21.onmicrosoft.com',
            type : 'GET',
            headers: {
                "accept": "application/json;odata=minimalmetadata",
                'Authorization': "Bearer" + "48076210176-JMswGJqMJ2d0eXHPnRN5A"
            },
            success : function(data) {              
                console.log(data)
            },
            error : function(request,error)
            {
                console.log("hi")
                console.log("Request: "+JSON.stringify(request));
            }
        })});
        </script>
    </head>    

    <body>
        hi
        <button></button>
    </body>
</html>
