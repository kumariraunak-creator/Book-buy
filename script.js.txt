function login() {
  let email = document.getElementById("email").value;
  let pass = document.getElementById("password").value;

  if (email === "" || pass === "") {
    alert("All fields required");
  } else {
    alert("Login Successful");
    window.location.href = "home.html";
  }
}

function goChat() {
  window.location.href = "chat.html";
}

function addItem() {
  alert("Item added successfully");
  window.location.href = "home.html";
}

function sendMsg() {
  let msg = document.getElementById("msg").value;
  if (msg !== "") {
    document.getElementById("chat").innerHTML += "<p>You: " + msg + "</p>";
    document.getElementById("msg").value = "";
  }
}
