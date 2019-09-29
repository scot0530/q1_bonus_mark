# q1_bonus_mark
  <script type="application/javascript">
    if (location.hostname === "localhost" || location.hostname === "127.0.0.1") {
        var validation = Cookies.get("validation");
        if (validation.length > 1) {
          var validation = Cookies.get('validation');
          document.getElementById('pageHTML').style.display = "block";
          document.getElementById('verificationString').innerHTML = validation;
          alert(window.atob(validation));
        }
    }
  </script>
  
  Hello Jose,
  My name is Duncan Scott and here is what I have come up with after our conversations during your office hours that you said you would give me the bonus for. Above is the code that reverses the implementation, to do it, I just had to delete the two characters in front of the alert(window.atob(validation)) line. I figured out that creating then checking for cookies was how the code checks it becasue of the string, and it was the window.atob() that decodes the base-64 encoded string, so I created the below code. Thanks for helping me to figure this out.
  Regards, Duncan
  
  <script>
function myFunction() {
alert(window.atob("TW96aWxsYS81LjAgKFdpbmRvd3MgTlQgMTAuMDsgV2luNjQ7IHg2NCkgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzc2LjAuMzgwOS4xMzIgU2FmYXJpLzUzNy4zNjo6aD03MjA6Onc9MTI4MDo6cGx1Z2luX25hbWU9Q2hyb21lIFBERiBQbHVnaW46OjQ1MDEwMDY0NjQ1MzczNjc2MDM4MDkxMzI1MzczNjM3MjAxMjgwMjQ="));
}
</script>
