# Tutoriais_Unity
Repository with basic unity components and scripts.
<ol>
  <li>Character Movement Trird Person</li>
  <p>
    using System.Colletions;<br>
    using System.Collections.Generic;<br>
    using UnityEngine;<br>
    <br>
    public class PlayerController : MonoBehaviour<br>
    {<br>
      //Camera<br>
      [SerializeField] Transform playerCamera = null;<br>
      [SerializeField] float mouseSensitivity = 3.5f;<br>
      <br>
      //Movimentation<br>
      [SerializeField] Float walkSpeed = 6.0f;<br>
      <br>
      //Gravity<br>
      [SerializeField] float gravity = -13.0f;<br>
      <br>
      //Smooth walk<br>
      [SerializeField] [Range(0.0f, 0.5f)] float moveSmoothTime = 0.3f;<br>
      [SerializeField] [Range(0.0f, 0.5f)] float mouseSmoothTime = 0.03f;<br>
      <br>
      //Jumping<br>
      floar jumpHeight = 3f;<br>
      <br>
      [SerializeField] bool lockCursor = true; //Lock the coursor in the middle of screen<br>
      <br>
      floar camera Pitch = 0.0f;<br>
      <br>
      //Gravity<br>
      float velocityY = 0.0f;<br>
      <br>
      CharacterController controller = null;<br>
      <br>
      Vector2 currentDir = Vector2.zero;<br>
      Vector2 currentDirVelocity = Vector2.zero;<br>
      <br>
      Vector2 currentMouseDelta = Vector2.zero;<br>
      Vector2 currentMouseDeltaVelocity = Vector2.zero;<br>
      <br>
      void Start()<br>
      {<br>
        controller = GetComponent<Character>();<br>
        if (lockCursor)<br>
        {<br>
          Cursor.lockState = CursorLockMode.Locked;<br>
          Curso.visible = false;<br>
        }<br>
      }<br>
      <br>
      void Update()<br>
      {<br>
        UpdateMouseLook();<br>
        UpdateMovement();<br>
      }<br>
    }<br>
  </p>
  <li>Tea</li>
  <li>Milk</li>
</ol>
