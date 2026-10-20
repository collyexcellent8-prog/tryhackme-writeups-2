import base64

def decode_brochure_flag(encoded_str):
    """Decode the Base64 string found in The Brochure challenge"""
    try:
        # The brochure hides data in Base64
        decoded = base64.b64decode(encoded_str).decode('utf-8')
        return decoded
    except Exception as e:
        return f"Error: {e}"

# Example from the room - you had:
# VEhNe1YzckBzX2FDQzB1bnRfaDRzX2IzM25fZjB1bmQhfQ==
# This decodes with CyberChef or python

if __name__ == "__main__":
    with open("encoded.txt", "r") as f:
        data = f.read().strip()
    print(decode_brochure_flag(data))
