# The 100% Proof Test
try {
    $response = Invoke-RestMethod -Uri "https://generativelanguage.googleapis.com/v1beta/models?key=AIzaSyBDC2Vz6mVtneCkmmaB2VtvftaxnyHSj6E"
    if ($response.models) { "✅ CONNECTION SECURE: Gemini API is fully reachable!" }
} catch {
    "❌ BLOCK DETECTED: Something is stopping the connection."
}
