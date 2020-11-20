```html
<!DOCTYPE html>
<html>
  <body>
    <form>

      <!-- Text Input -->
      <label>First Name:</label>
      <input required type="text" name="firstName" id="firstName">
      <!-- That's bad M'kay -->
      <!-- <br><br><br><br><br><br><br><br><br><br><br><br> -->
      <br>
      <label>Last Name:</label>
      <input pattern=".{3,}" type="text" name="lastName" id="lastName"><br>
      <br>

      <!-- Date Input -->
      <label>Date of Visit</label><br>
      <input disabled type="date">
      <br><br>

      <!-- Radio Button Input -->
      <label>What Restraunt did you eat at?</label><br>
      <input type="radio" name="restaurant" value="nyc"><label>NYC</label><br>
      <input type="radio" name="restaurant" value="LA"><label>LA</label><br>
      <input type="radio" name="restaurant" value="wilmington"><label>Wilmington</label><br>
      <br>

      <!-- Checkbox Input -->
      <label>What meal did you order</label><br>
      <input type="checkbox" name="meal1" value="breakfast"><label>Breakfast</label><br>
      <input type="checkbox" name="meal2" value="lunch"><label>Lunch</label><br>
      <input type="checkbox" name="meal3" value="dinner"><label>Dinner</label><br>
      <input type="checkbox" name="meal4" value="appeitizer"><label>Appeitizer</label><br>
      <input type="checkbox" name="meal5" value="dessert"><label>Dessert</label><br>
      <br>

      <!-- Dropdowns -->
      <label>Rate your Experience:</label>
      <select name="rating">
        <option value="1">1</option>
        <option value="2">2</option>
        <option value="3">3</option>
        <option value="4">4</option>
        <option value="5">5</option>
      </select>
      <br><br>

      <!-- Text Area -->
      <label>Comments</label><br>
      <textarea name="comments" cols="10" rows="4" maxlength="10"></textarea>
      <br><br>

      <button>Submit</button>
    </form>
  </body>
</html>
```